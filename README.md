# springboot-shiro-demo
copy自纯洁的微笑
1、编写好后就可以启动程序，访问http://localhost:8080/userInfo/userList页面，由于没有登录就会跳转到http://localhost:8080/login页面。登录之后就会跳转到index页面，登录后，直接在浏览器中输入http://localhost:8080/userInfo/userList访问就会看到用户信息。上面这些操作时候触发MyShiroRealm.doGetAuthenticationInfo()这个方法，也就是登录认证的方法。

2、登录admin账户，访问：http://127.0.0.1:8080/userInfo/userAdd显示用户添加界面，访问http://127.0.0.1:8080/userInfo/userDel显示403没有权限。上面这些操作时候触发MyShiroRealm.doGetAuthorizationInfo()这个方面，也就是权限校验的方法。
