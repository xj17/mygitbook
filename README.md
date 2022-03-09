随手一记

关于端口占用：

根据端口号查询出对应的进程号，然后杀死该进程。

netstat -ano|findstr ‘端口号’

taskkill /pid ‘进程号’-f

------

ajax之async属性

async:默认值是true,所有请求为异步请求。如果需要发送同步请求，需要将此项值设为false。

