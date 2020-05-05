# Community
个人练习项目, 本项目实现了一个多用户发帖评论的社区平台。实现了邮箱注册、验证码登录、发帖、评论、私信、点赞、关注、统计网站访问次数、全文搜索等功能。使用SpringBoot, MyBatis,Thymeleaf开发,数据库使用MySQL和Redis，使用Kafka实现异步消息，使用Elasticsearch实现全文搜索功能。
## 演示
本项目部署在阿里云ECS服务器上,演示地址  http://community.closedonsunday.top  (演示用户名:guest 密码:guest)
 
  

 
## 主要技术
 
### Redis
    1.保存用户登录状态,代替Session
    2.缓存用户信息,减少数据库访问
    3.存储关注和点赞数据
    4.临时保存验证码
    5.统计网站每天的访问次数
### Kafka
    * 实现异步消息,异步通知用户收到的点赞,关注,私信
### Elasticsearch
    * 实现全文搜索功能. 同步帖子数据,对帖子的标题和正文建立倒排索引,实现全文搜索

    
    
