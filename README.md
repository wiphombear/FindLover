﻿FindLover
=========

仿花田网，内部相亲网站 基于Asp.Net MVC3 Bootstrap2 Juqery1.7.2

1.先设置数据库：
  在Models--LoveDb.cs中 设置你的连接字符串，我没有写入webconfig。支持数据迁移。

2.需要自己再注册

3.管理员自己再数据库中添加，权限部分不是很全面。
  
  需要在Roles表中 将自己加为SysAdmin 

  Id    UserId  RoleType         ActionTime
  1	1	SysAdmin	2013-08-10 21:24:23.370

 还有在Authorities表中，加入权限

  1	1	True	True	True	True	True

  AdminStatistics 是用来统计管理员的操作数据的。加上自己的。

  你都可以自己完善或者扩展。

4.Helper文件夹中的SendMail 类 改成你自己的服务器和邮箱 不用也可以拿掉。
  在用户注册，举报，上传头像会mail通知的。
----------------------------------------------------------------------------------------
可能的问题：
 1.上传头像和上传图片在ie家族中是有问题的  建议用chrome打开
 2.Topic 发布用的是kendoui，修改的时候会有bug。 这个问题需要用一个隐藏的div转换一下。
 3.这个版本没有加分页处理，同志们可以自己加分页。
 4.不足之处还很多，用户主页在某些ie8浏览器下 图像右边是空白的，我还没找到原因。

----------------------------------------------------------------------------------------- 
这个版本供大家学习，本身技术细节上没有什么亮点，满足大家的好奇心。特此分享给大家
 
 更详细的一些细节请参考我的博客。