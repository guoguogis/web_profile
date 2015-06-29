### 统计网页加载性能

#### 网页性能统计指标有：

> 白屏时间： 头部外链资源加载完成,通过在head尾标签中添加时间戳的方式来实现；

> 首屏时间： 通过统计首屏的图片/iframe的加载时间来确定，即在所有统计的时间中筛选出最长的时间；

> 可操作时间： 一般通过统计domready的时间来评估可操作时间，对于模块化异步加载的场景需要在特定的js加载成功后自定义时间点。

> 总加载时间： 一般通过onload的时间来评估总加载时间，如果页面有比较多的ajax请求，则通过ajax请求结束的时间来评估。

#### 数据库设计

> ##### 实时性能表 current_perf：

> explore_name         浏览器名称

> os_name              操作系统名称

> current_time         时间

> black_waiting_time   白屏时间

> fist_page_time       首屏时间

> operation_time       可操作时间

> total_time           总加载时间


