#基本信息
---
<img src="./img/tou.png" style="float:right;">

刘悦 1994年6月（注意和你包装后的年龄要吻合,另外讲师必须放照片，最好是艺术照，本人的）

3年工作经验

手机：134-333-29111

邮箱：123@gmail.com  (建议用gmail)

个人网站:v3u.cn

##个人简介(注意技术点要高亮)
---
3年互联网从业经历，科班出身，深厚的数据结构和算法基础，动手能力强，熟练使用后端**Tornado**框架以及前端**vue.js**，对互联网技能培训有自己的见解和感悟。持有英语专业四级证书（TEM-4），有海外工作经验，一流的沟通能力，多次组织并参与内部培训与技术分享，多次参与美国麻省理工学院（MIT）线上直播分享，熟练掌握**Scratch3.0**，对少儿编程具备一定前瞻性了解。


#少儿编程（自我介绍）
您好，我是15年毕业的，毕业之后本来准备考研，后来机缘巧合来到北京实习了一年左右，之后就留在了北京在一家创业型团队（小公司）起步，一直使用python作为开发语言，在公司里也是一直和业务打交道，沉淀了大约一年左右，我跳槽到了（你主要包装的第二家大厂），薪酬实现了double，在新的技术团队里，我接触到了vue框架，体会到了数据双向绑定这种先进的理念，同时由于前后端都参与开发（微信小程序），技术栈也越来越丰富，最近半年我在公司一直负责组织团队技术分享和新员工技术培训以及一些新技术的预研，因为我们公司在东南亚也有分公司，其中一个base在吉隆坡，所以我经常从北京直飞吉隆坡组织技术分享会，在分享会里我接触到了MIT（美国麻省理工）开发的一款面向青少年编程软件SCRATCH，我对这个软件非常感兴趣，同时也觉得很有意思，由于少儿编程在我国处于刚刚起步的阶段，我感觉很多人对少儿编程有很多误解，其实呢，让小朋友学编程并不是就是说以后要去做程序员，而是培养一种冷静和逻辑化的思维，我个人认为思维模式和思考问题的方法是尤为重要的，因为很多adults(成年人)基础教育和家庭教育等等原因导致容易形成很多思维定式，这在工作和学习中会对他们造成障碍，所以在青少年时期就培养逻辑化思维有助于人们成年后有更好的发展。我个人来讲，优势就是技术涉猎比较广，前后端都接触过，另外沟通能力和理解能力比较强，在跨国企业的经历也让我乐于分享，并且我一直保持着写技术博客的习惯，这样也可以结交更多的国际友人，我的介绍完了，thanks。

##教育经历
---
2012.08 - 2016.06 北京电子科技大学通信工程学院 统招一本

##技能列表（内容不宜太多，突出重点，没用过不懂的不要写，熟练程度由左至右）
---
* 后端框架：Tornado
* 前端框架：Vue.js
* 数据库：MySQL,Redis
* 工具：Docker,Git,Excel
* 其他：微信小程序/公众号开发，Tensowflow
* 外语：TEM-4，能流畅阅读英文文档，口语沟通无障碍

##工作经历
---

* 2018年7月 - 至今
钱方好近(北京)科技有限公司—高级项目经理

* 2016年9月 - 2018年5月
北京谐云科技有限公司—初级python开发工程师

##近期参与项目（顺序为倒序，最新的项目排第一位，同时第一位也是你的主力项目，你必须熟悉能说，并且知识点要全，同时项目之间的时间点要连起来，不要断开）
---

###主导钱方好近移动聚合支付平台开发(2019年1月-2019年8月)

项目简介：解决商户与各个支付平台复杂的支付逻辑，统一支付码，不通过现金结算即可按照商户需要展开个性化定制，利用与各第三方支付平台以及合作银行等的聚合，所开展的一项支付工具多样化的综合支付业务

* 基于**Tornado**实现**Restful**风格的在线聚合支付接口，聚合封装了支付宝，微信，京东等三方支付平台
* 使用**Mysql**存储数据，配置主从热备，水平分表。
* 采用**Celery**和**Rabbitmq**异步任务队列架构，同时配置自动化定时任务
* 利用**Websocket**实现后端消息主动推送，改造前端传统轮询技术框架，**减少了30%的网络请求数**，节约了大约一半的可用带宽
* 使用**Redis**集群作为缓存介质，缓解数据库压力。
* 利用**Docker**进行服务封装和业务解耦，使用**Docker-compose**批量管理容器集群，用**Docker-file**编写部署脚本
* Nginx反向代理Tornado，采用加权策略的负载均衡技术，后台服务统一使用**SuperVisor**进行管理
* 利用**gensim**对用户投诉及评论信息进行模糊匹配与情感分析，预测用户导向。
* 后期使用**Thrift**框架RPC协议架构对传统的http接口进行重构，提高了整体接口的性能和吞吐量。
* 使用**Redisearch**打造全文检索引擎，百万级数据可以达到单次检索10毫秒以内的速度。
* 利用**FastDFS结合FastDHT**实现用户上传文件的分布式去重存储。
* 开发，测试用户认证，订单，支付/退款等7个模块


###参与宝宝树线上产品功能的预研和开发测试

项目简介：宝宝树是一款以书籍形式记载宝宝成长，交流育儿心得的产品。包含五大模块，成长书，交流，服务，商城和我。涵盖功能为书籍行事记录宝宝点滴，发帖沟通交流，线上求助咨询和线下亲子活动，网上商城购买宝宝用品。

* 




###主导分布式短视频抓取爬虫系统(2018年6月-2018年12月)

* 作为组长负责设计和开发基于**Scrapy**的分布式短视频抓取系统，优化爬虫策略和防屏蔽规则,利用**Redis**维护ip代理池，提升短视频抓取的效率和质量。
* 使用**Jenkins**自动化部署服务，提高系统可用性
* 使用**Go lang**对抓取框架进行重构，提高了**200%的爬虫效率**
* 利用**Docker**对项目进行重新拆分和架构，减少项目模块之间的资源耦合度，实现了持续集成
* 使用**MarkDown**编写公司技术文档以及维护，定期review团队的代码，与团队成员共同进步
* 使用**Selenium**和**puppeteer**针对反爬虫进行反复测试和改进抓取方案
* 整合微信，微博，qq等多个三方登录平台，打造一键式社交账号绑定系统，提高用户体验


###参与移动聚合支付后台管理系统(CMS)(2018年6月-2018年12月)

* 基于**Tornado**的后台管理平台，采用**RBAC**权限管理机制
* 利用**Jieba分词模块**对商户进行打标签操作，使用**Mongodb**存储标签数据
* 使用**Supervisor**对后台服务例如**uwsgi**和**Gunicorn**进行监控和操作，**降低了日常维护成本**
* 使用**Redis**作为缓存介质，利用其分布式锁和队列的特性开发并测试抢单秒杀功能


###参与在线视频监控直播平台(以SaaS服务为核心，向客户提供操作简便适用于多场景的云直播平台)(2018年1月-2018年6月)

* 搭建基于**Docker**挂载**Nginx-rtmp**的直播服务器
* 使用**FFmpeg**利用客户端设备进行推流，对视频进行**头图提取，精华片段转换动图，视频埋点，视频信息分析**等操作
* 开发，测试点播，直播，播单等7个模块
* 采用**FastDfs**分布式文件系统作为海量视频存储方案，利用**视频指纹**规避重复文件问题,节约了**大约20%的硬盘空间**
* 在网页端使用**vue.js**作为载体利用**video.js**作为直播流播放器，**优化延迟达到500ms左右**
* 利用**Nginx**反向代理后台**uwsgi+Django**的点播接口，并且针对性使用Nginx**负载均衡**策略
* 使用**Bootstrap**作为播放页响应式设计解决方案，一套代码自适应大小屏应用，**降低了50%左右的移动端开发成本**


###独立开发自动化运维工作流平台(devops)(2017年6月-2017年12月)

* 对日常上线工作流标准化精简化，构建 **上线工作流提交——》审批——》测试回归-》灰度回归-》生产环境-》PM回归-》工作流结束** 完整的标准化流程，减少了线上事故发生的几率。
* 集成**jenkins**，将冗长的代码拉取，合并分支等操作转化为一键式的部署。
* 开发资产管理模块，对测试，灰度，生产各种环境下的服务器有效的管理和分配，定期监控服务器运行状态。
* 采用**响应式设计**前端框架，方便Leader随时审批和查看平台状况。
* 集成**Supervisor**，将后台服务状态可视化，简化服务操作。

##兴趣与奖项
---

崇尚极客文化与开源精神，具有海外工作经验(base:吉隆坡)

活跃在stackoverflow等技术论坛，热衷解决问题和探索

跟随团队参与2019年WeChat Developer Challenge微信开发者大赛新加坡站，并获荣誉奖


#学编程并不是就是说以后要去做程序员，而是培养一种冷静和逻辑化的思维
