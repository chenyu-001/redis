# redis
use redis
#Ubuntu配置redis报错adlist.0

更新过各种软件包之后仍报错
是因为默认的redis默认编译与linux不同，要强制编译redis使用libc malloc，使用: make malloc=libc 指令//借用
