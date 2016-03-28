IntilliJ IDEA 儲存SVN帳密的方法

# [IntelliJ IDEA 10.5 on Mac OS X: save subversion credentials](https://mihail.stoynov.com/2011/06/20/intellij-idea-10-5-on-mac-os-x-save-subversion-credentials/)

#### This is a note-to-self. So when I forget the solution I can come back here and find it.

#### IntelliJ IDEA is one of the best Java IDEs. More [here](http://www.jetbrains.com/idea/).

I have had the problem of not being able to save the password of a test svn repository. I found the solution:

```
- vi ~/.subversion_IDEA/servers
- add the following lines:
store-passwords = yes
store-plaintext-passwords = yes
- Save and restart Idea.
- Play around with the changes tab until a popup shows up that asks for credentials.
- Give the credentials and click <Save the credentials> or whatever it says.
- That's it.
```
