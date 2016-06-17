terminal 連線指令：
```
sudo ssh ubuntu@ec2-52-196-215-165.ap-northeast-1.compute.amazonaws.com -i ~/ec2-keys/id_jason90929.pem
```

剛建立好環境時所需步驟

進入 root：
```
sudo -i
```

更改時區：
```
dpkg-reconfigure tzdata
```

更新 apt-get：
```
apt-get update
```

安裝 Nginx：
```
apt-get install nginx
```

Nginx 啟動、關閉、重啟：
```
service nginx start
service nginx stop
service nginx restart
```

檢查 Port 80 是否已開啟：
```
netstat -ant | grep :80
```

開啟 Port 80：
```
iptables -A INPUT -p tcp --dport 80 -j ACCEPT
```

Nginx 放置網頁的資料夾路徑：
```
cd /usr/share/nginx/html
```

開啟 Nginx 的路徑設定，關鍵要把靜態網頁的存放位置放對：
```
vi /etc/nginx/conf.d/default.conf
```

default.conf 的設定：
```
server {
    # 這個虛擬主機的 Port 和名稱
    listen 80;
    listen [::]:80;
    server_name  localhost;
    root /home/ubuntu/www/jason-tseng;
    index  index.html index.htm;

    # 預設編碼，但通常不建議開啟，讓網頁中的 meta 或 header 自行定義
    #charset koi8-r;

    # 可以額外針對這個站台修改 log 的存放位置
    #access_log  /var/log/nginx/log/host.access.log  main;

    # Make site accessible from http://localhost/
    server_name *.amazonaws.com;

    # 根目錄的設定
    location / {
        # 實際的檔案位置
        # root   /usr/share/nginx/html;
        # 預設首頁檔名
        # index  index.html index.htm;
    }

    location ~* \.(?:ico|css|js|gif|jpe?g|png|ttf|otf)$ {
        expires 30d;
        add_header Pragma public;
        add_header Cache-Control "public";
    }

    # 如果發生 404 可以指定到特定的頁面來顯示
    #error_page  404              /404.html;

    # redirect server error pages to the static page /50x.html
    #
    error_page   500 502 503 504  /50x.html;
    #location = /50x.html {
    #     root   /usr/share/nginx/html;
    #}

    # proxy the PHP scripts to Apache listening on 127.0.0.1:80
    #
    #location ~ \.php$ {
    #    proxy_pass   http://127.0.0.1;
    #}

    # pass the PHP scripts to FastCGI server listening on 127.0.0.1:9000
    #
    #location ~ \.php$ {
    #    root           html;
    #    fastcgi_pass   127.0.0.1:9000;
    #    fastcgi_index  index.php;
    #    fastcgi_param  SCRIPT_FILENAME  /scripts$fastcgi_script_name;
    #    include        fastcgi_params;
    #}

    # deny access to .htaccess files, if Apache's document root
    # concurs with nginx's one
    #
    #location ~ /\.ht {
    #    deny  all;
    #}
}


```



設置檔案到期日
```
location ~* \.(?:ico|css|js|gif|jpe?g|png|ttf|otf)$ {
    expires 30d;
    add_header Pragma public;
    add_header Cache-Control "public";
}
```

之後就在這個頁面丟上整包網站：
```
cd /home/ubuntu/www/jason-tseng
```

並且在 AWS Security 端打開  TCP 80，就可以對外了

[Security 要開啟對外的 80 TCP](http://serverfault.com/questions/471133/deploying-a-static-site-on-aws-ec2-nginx-what-am-i-doing-wrong)
