### Linux中几种IO模型，有哪些区别？

答：select、poll、epoll

> https://www.jianshu.com/p/486b0965c296

> https://blog.csdn.net/baiye_xing/article/details/74331041



### Linux的top下的buffer与cache的区别

**buffer:**

  缓冲区，一个用于存储速度不同步的设备或优先级不同的设备之间传输数据

的区域。通过缓冲区，可以使进程之间的相互等待变少，从而使从速度慢的设备读入数据

时，速度快的设备的操作进程不发生间断。

**cache:**

   当你读写文件的时候，Linux内核为了提高读写性能与速度，会将文件在内存中进行缓存，

这部分内存就是Cache Memory(缓存内存)。即使你的程序运行结束后，Cache Memory也不会

自动释放。这就会导致你在Linux系统中程序频繁读写文件后，你会发现可用物理内存会很少。

其实这缓存内存(Cache Memory)在你需要使用内存的时候会自动释放，所以你不必担心没有

内存可用。如果你希望手动去释放Cache Memory也是有办法的



### 常见Linux命令是否用过，比如strace和netstat

