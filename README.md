#把书读薄之《Advanced Programming in the Unix Environment》

##前言
既然读书，就把它读薄。  
在学习C语言的时候我读到过一句话，说C语言并不是个复杂的语言，因此介绍C语言的书没必要太长。我觉得很合心意，然后就喜欢上这个语言——谁会不喜欢简洁的设计呢？  
但并非所有的语言或设计都是如此，比如操作系统， 它本身就是个庞大复杂的家伙，是许多人协作劳动的成果并充满了繁多的细节。幸运的是有一种人有提炼总结的特异功能，能像炼金术士一样把知识归纳总结重新浓缩提炼，再次呈现出来的时候不失原味又井井有条，所有的学习者都因为他们的智慧受益。W. Richard Stevens就是这样的炼金术士，他的《Advanced Programming in the Unix Environment》和《UNIX Network Programming》都是了不起的创造和作品。我崇拜这样的人。  
可即便如此，《Advanced Programming in the Unix Environment》也有1000页，这是因为本质上是手册类的书籍需要面面俱到，容纳各种细节和特例。但作为学习者的普通人类显然是无法将所有知识都记忆的，当然也没有必要。好的学习者阅读一本书的过程应该是自己构建起知识索引，能够快速的回忆和应用，所谓消化知识就是这个意思。  
这里的把书读薄系列就是我阅读过程中试图建立的大脑索引，它抽取了一部书（或一个领域）中最重要的方面，将每一个方面通过一幅图或者文字脉络将重要（运用频繁）的知识串起来，而舍弃掉置业上的一些细节和特例。当然既然你已经构建起了知识的全景，你自然知道取哪里找到这些细节和特例。  
总而言之，这是个人的读书笔记。只不过我努力将它写的对阅读者友好，而不论阅读者是别人还是自己——就像程序注释那样。  




##纲要
简单说来，Unix环境给程序员提供的就是一系列的系统调用(System Call)和C库函数(C Library Function)，程序员通过在程序中调用这两者来使用操作系统的服务。因此本质上学习《Advanced Programming in the Unix Environment》就是学习这些系统调用(System Call)和C库函数(C Library Function)，但如果认为《Advanced Programming in the Unix Environment》仅仅是一本接口手册，就有点儿买椟还珠了。这本书的经典之处就在于它不仅把这些接口函数的讲解分门别类，描绘了接口背后Unix系统的相关设计和原理，在辅以了丰富的实例代码来展示怎样使用这些接口，与一般的手册可谓是云泥之别。  

我认为Unix环境编程的知识最重要的就4个方面，这4个方面占了Unix环境编程知识中的80%以上，掌握之后基本认为对Unix系统胸有成竹了。它们是：
- 文件系统 (File System)
- 权限控制 (Permission Control)
- I/O (包括Buffered I/O 和 Unbuffered I/O)
- 进程和线程 (Process & Thread，包括进程控制，线程控制，进程间通信(socket也是其中之一))

除取上面4个方面，剩下的内容不多，可以很快扫尾，我统称为“其他”：
- 信号 (Signal)
- 时间 (Time)
- 错误处理 (Error Handle)
- 内存分配和管理 (Memory Allocation and Management)




##Section 1: 文件系统 (File System)

待整理：  
1. Unix的文件系统由目录和文件构成树状结构。  
   目录结构中每个条目由文件名和inode号构成  
   inode中存了权限，文件大小，用户ID，组ID，文件类型等信息  
2. link文件，硬链，软链（符号链）  




##Section 2: 权限控制 (Permission Control)

待整理：  
1. user ID，group ID，supplementary group ID——/etc/passwd  
2. 进程的real userID，real groupID  
         effective userID， effective groupID  
3. open方式指定，以及文件的读写执行权限  




##Section 3: I/O (包括Buffered I/O 和 Unbuffered I/O)

待整理：  
1. 打开文件之后的内存图（process talbe -> file talbe -> v-node table）  
2. open read write lseek close  




##Section 4: 进程和线程 (Process & Thread，包括进程控制，线程控制，进程间通信(socket也是其中之一))

待整理：  
1. process ID  
2. thread ID（thread ID只在特定线程中有意义）  
3. 进城控制: fork exec waitpid  




##Section 5: 其他 

待整理：  
- 5.1信号 (Signal)  

- 5.2时间 (Time)  
自1970年以来的时间  
进程时间（1. clock time 2. user CPU time 3. System CPU time）  

- 5.3错误处理 (Error Handle)  
变量errno（nerver equal zero）—— <errno.h>  
函数strerror  
函数perror  

- 5.4内存分配和管理 (Memory Allocation and Management)  




待考虑：  
p2 Figure 1.1 Architecture of the UNIX operating system  
