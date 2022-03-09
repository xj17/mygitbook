1.由于springboot提供的自动配置功能十分丰富，自动配置的功能可能不符合我们的需求，需要我们自定义配置，这个时候需要我们排除springboot的某些配置

以redis来举例

通常有两种方法将其关闭

***第一种:***

在yml或properties文件中配置

比如application.properties文件中添加spring.autoconfigure.exclude=org.springframework.boot.autoconfigure.data.redis.RedisAutoConfiguration

然后再对应的bean上 添加 @Autowired(required=false)，表示忽略当前要注入的bean。

***第二种:***

使用 @SpringBootApplication 注解的时候，使用 exclude 属性进行排除指定的类：

比如@SpringBootApplication(exclude = {  RedisAutoConfiguration.class })

~~RedisRepositoriesAutoConfiguration 对 beanName 叫做 “redisTemplate” 的bean有依赖，需要一并排除~~