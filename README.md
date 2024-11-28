# Monitoring
病毒木马监控辅助工具

红蓝队监控辅助工具
1、工具介绍
此工具是监控一些常见的病毒、Webshell、计划任务、服务等。
可与前面的流量工具结合使用，两个工具没整合到一起。
https://www.bilibili.com/video/BV1WRxseYETt/?vd_source=229f70258c44853078f16a5decbc2fb0

 ![图片](https://github.com/user-attachments/assets/bbba6af2-8b2e-43f8-a771-1ad516e5d053)


2、适用场景
(1)、红队：主要是防止被Github、某某公众号、星球等上的开源(闭源)工具有意或无意的投毒。
(2)、蓝队：攻防对抗演练护网期间使用，适合于裸奔的客户。

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

 

