**主要问题**：现在有个爬虫程序摆在我面前，它长时间爬着爬着爬虫程序和数据库的内存就会增大，因影响爬虫的继续和电脑或服务器的正常使用。

**解决思路**： 
* 1. 通过判断cpu 和内存占用率 然后决定是否要杀死爬虫程序和数据库服务进程
* 2. win下 通过 tasklisst 命令获取到我们需要的pid 然后杀死进程
* 3. 重启爬虫程序和数据库
* 4. 做个时间延迟并循环判断