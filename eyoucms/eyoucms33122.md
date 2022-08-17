BUG_Author：朝歌
Software Link : https://github.com/eyoucms/eyoucms
Website : http://www.eyoucms.com/
Vulnerable version 1.5.6 download address ：https://www.eyoucms.com/plus/down.php
After the installation is complete, log in as admin, open the page
[![Xgf7RO.jpg](https://s1.ax1x.com/2022/06/12/Xgf7RO.jpg)](https://imgtu.com/i/Xgf7RO)
Here you can fill in malicious JavaScript code to cause stored xss
[![XgfOLd.png](https://s1.ax1x.com/2022/06/12/XgfOLd.png)](https://imgtu.com/i/XgfOLd)
Malicious code is spliced ​​into the href link
[![Xgfxot.jpg](https://s1.ax1x.com/2022/06/12/Xgfxot.jpg)](https://imgtu.com/i/Xgfxot)
Causes stored XSS to steal sensitive information of logged-in users
[![XghnYV.png](https://s1.ax1x.com/2022/06/12/XghnYV.png)](https://imgtu.com/i/XghnYV)
POC :
```Plaintext
javascript:alert(/XSS/)
```
