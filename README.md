# spring-cloud-demo
springcloud skywalking mqtt  demo


1. spring-cloud and skywalking demo
2. add mqtt suports
3. add 微信小程序 suports mqtt
4. kafka elk支持



20180809
1. 更新 代码结构
2. 新增git配置中心
3. 新增kafka elk demo配置以及文档
4. 文档结构整理
5. 分离注册中心和配置中心
7. 添加zipkin服务跟踪


20180905
1. 自定义注解实现aop日志
2. 自定义注解实现实体类参数校验
3. 添加mybatis自定生成映射实体类、mapper等
4. 添加全局异常处理
5. 添加fegin自定义数据解析

20180907
1. 添加注解，作为参数校验入口

20180910
1. 解决服务之间调用fegin+hystrix 熔断异常拦截处理

20180914
1. 服务调用之间的rest请求，参数为对象时需要添加@RequestBody注解
```eg:
```saveRegionCity(@RequestBody RegionCityDto regionCityDto)
2. 服务间调用接口的返回值，不能使接口返回，必须要使用实现类返回，fegin客户端获取不到数据返回Null
```eg:
``` public User getUser(@RequestBody UserQuery query);-User必须为实现类，不能为接口
3. 添加fastjson解析，解决部分调用对象内包含对象传值为空问题


