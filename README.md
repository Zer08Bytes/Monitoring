# Monitoring

红蓝队监控辅助工具介绍：

此工具不是杀毒软件、不是杀毒软件、不是杀毒软件。

此工具是一个辅助监控工具(特殊场景和人员使用，见下面的适用场景)，监控一些常见的病毒文件类型、Webshell、计划任务、服务等。 


https://www.bilibili.com/video/BV1WRxseYETt/?vd_source=229f70258c44853078f16a5decbc2fb0

 ![图片](https://github.com/user-attachments/assets/bbba6af2-8b2e-43f8-a771-1ad516e5d053)


1、视频操作手册：
本视频。




2、适用场景：

(1)、红队：主要是防止被Github、某某公众号、星球等上面的开源(或闭源)工具有意或无意的投毒。

(2)、蓝队：攻防对抗演练、护网期间使用，特别适合于裸奔的客户。

(3)、病毒分析人员：调试分析病毒木马期间，监控释放的文件、创建的服务等等。


3、监控的内容：

1）默认监控常用病毒木马落地磁盘的类型

默认监控的文件类型已经内置。

2）默认监控的Webshell类型有如下：
'.asp', '.asa', '.cer', '.cdx', '.htr', 'cfm', '.stm', '.shtm', '.shtml',
'.aspx', '.asax', '.ashx', '.ashm', '.asmx', '.ascx', '.svc', '.soap', '.cshtml', '.config',
'.php', '.php2', '.php3', '.php4', '.php5', '.phps', '.phtml', '.pht', '.php::$DATA', ".htaccess",
'.jsp', '.jspx', '.jspf','.jspa', '.jsw', '.jsv', '.jtml', "war"

如果上述webshell类型还不能满足，用户可以去自定义添加，比如添加.abc文件后缀，那样就会同时监控上述类型和用户自定义的.abc类型。

3）默认监控 计划任务的创建和修改

4）默认监控 windows服务的创建和修改



3、工具监控截图(每个部分都有单独的日志留存)

 ![图片](https://github.com/user-attachments/assets/8336de7b-ac1d-4bc6-9a37-2f319543b110)
 

![图片](https://github.com/user-attachments/assets/8c1a3556-e08b-4a07-80a5-606da8a44b1e)


 ![图片](https://github.com/user-attachments/assets/14d760fc-24bc-4cca-bf68-b564d3f7b08c)
 

![图片](https://github.com/user-attachments/assets/1b263244-78bd-4c94-8cad-53533b8e2e8c)

4、同步日志(为溯源提供帮助)

日志信息同步网络空间其他的主机(比较实用，防止被入侵后，清除了日志，包括系统日志也可以同步)

这里采用单向同步且启用版本控制，防止日志被覆盖。

推荐工具（不是做广告哈~）

简单介绍一下设置：

被同步端设置(也就是需要把日志上传到其他主机的一端)：


 ![图片](https://github.com/user-attachments/assets/d08f9550-6138-4e3f-acde-b2dfdc684c92)
 

![图片](https://github.com/user-attachments/assets/4f496f7d-1e6f-4676-83b0-13068874a0d3)
 

同步端设置(也就是远程备份日志的主机端)：

 ![图片](https://github.com/user-attachments/assets/ee79c00b-5aef-40be-a573-81ef5354ad49)
 

![图片](https://github.com/user-attachments/assets/c2aab64b-fd17-4aeb-9afa-63b09b533b49)


![图片](https://github.com/user-attachments/assets/5d041ed3-a839-4f43-b723-f2507bcbb271)


![图片](https://github.com/user-attachments/assets/aff62619-9b95-41ec-9106-724205006f2c)



同步过来的日志文件，且有版本控制
 
![图片](https://github.com/user-attachments/assets/d745ca6c-55b8-4c64-95c3-710d109600c4)


![图片](https://github.com/user-attachments/assets/81518563-a5fe-46cd-8306-2c253dc9d82a)

 
PS:

1、由于本人水平有限，目前未能实现对注册表的监控。 计划未来版本新增注册表的监控。如有大佬会的，请私我，感谢。

2、建议使用管理员权限运行本程序。

3、代码写的烂，写的仓促，还有许多需要优化的地方，放在下一个版本中解决吧。

4、小"彩蛋"：在监控过程中，不需要停止任务，可以随时添加需要监控的Webshell后缀。

5、后期打算给程序加一个防止结束本进程的功能，有大佬有现成代码的，请私我，感谢！


