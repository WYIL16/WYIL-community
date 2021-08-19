# WYIL-community
牛客社区成品代码   技术栈：Spring Boot+MyBatis+MySQL+Redis+Kafka+Elasticsearsh  
工作内容：  • 使用Redis存储和登陆ticket和验证码，解决分布式session问题，同时实现发帖，评论，私信等社区功能； 
• 使用Redis的set实现点赞，zset实现关注，Hyper log log统计UV，Bitmap统计DAU； 
• 使用Kafka处理发送评论、点赞和关注等系统通知，起到解耦和异步调用的作用； 
• 使用Elasticsearsh对帖子搜索功能进行重构，通过IK中文分词器增加索引和全局索引，实现搜索关键字高亮显示等功能；
• 对热帖排行模块，使用分布式缓存Redis和本地缓存Caffeine作为多级缓存，将QPS提升了20倍（10-200），大大提升了网站访问速度，并使用Quartz定时更新热帖排行榜；
