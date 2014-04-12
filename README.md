##把书读薄之《Advanced Programming in the Unix Environment》

####前言
既然读书，就把它读薄。  
在学习C语言的时候我读到过一句话，说C语言并不是个复杂的语言，因此介绍C语言的书没必要太长。我觉得很合心意，然后就喜欢上这个语言——谁会不喜欢简洁的设计呢？  
但并非所有的语言或设计都是如此，比如操作系统， 它本身就是个庞大复杂的家伙，是许多人协作劳动的成果并充满了繁多的细节。幸运的是有一种人有提炼总结的特异功能，能像炼金术士一样把知识归纳总结重新浓缩提炼，再次呈现出来的时候不失原味又井井有条，所有的学习者都因为他们的智慧受益。W. Richard Stevens就是这样的炼金术士，他的《Advanced Programming in the Unix Environment》和《UNIX Network Programming》都是了不起的创造和作品。我崇拜这样的人。  
可即便如此，《Advanced Programming in the Unix Environment》也有1000页，这是因为本质上是手册类的书籍需要面面俱到，容纳各种细节和特例。但作为学习者的普通人类显然是无法将所有知识都记忆的，当然也没有必要。好的学习者阅读一本书的过程应该是自己构建起知识索引，能够快速的回忆和应用，所谓消化知识就是这个意思。  
这里的把书读薄系列就是我阅读过程中试图建立的大脑索引，它抽取了一部书（或一个领域）中最重要的方面，将每一个方面通过一幅图或者文字脉络将重要（运用频繁）的知识串起来，而舍弃掉置业上的一些细节和特例。当然既然你已经构建起了知识的全景，你自然知道取哪里找到这些细节和特例。  
总而言之，这是个人的读书笔记。只不过我努力将它写的对阅读者友好，而不论阅读者是别人还是自己——就像程序注释那样。  

####纲要
Unix环境编程的知识我认为最终要的就4个方面:  
- 文件系统 (File System)
- 权限控制 (Permission Control)
- I/O (包括Buffered I/O 和 Unbuffered I/O)
- 进程和线程 (Process & Thread 包括进程控制，线程控制)
这4个方面占了Unix环境编程知识中的80%以上，掌握之后基本认为对Unix系统胸有成竹了。  

除取上面4个方面，剩下的内容不多，可以很快扫尾，我统称为“其他：
- 信号 (Signal)
- 时间 (Time)
- 错误处理 (Error Handle)
- 内存分配和管理 (Memory Allocation and Management)
