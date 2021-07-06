# StringBuffer和StringBuilder的区别

StringBuffer：

StringBuffer 线程安全的可变字符序列。如果要频繁对字符串内容进行修改，出于效率考虑最好使用 StringBuffer。在任意时间点上它都包含某种特定的字符序列，但通过某些方法调用可以改变该序列的长度和内容。可将字符串缓冲区安全地用于多个线程。可以调用 StringBuffer 的 toString() 方法转成 String 类型。

StringBuilder：

StringBuilder 对象被当作是一个包含字符序列的变长数组。StringBuilder兼容StringBuffer的 API但不保证同步。该类被设计用作 StringBuffer 的一个简易替换，用于字符串缓冲区单线程场景。

使用场景：

1. 操作少量的数据用String ,单线程操作大量数据，多线程操作大量数据用StringBuffer。

2. 避免使用"+"来对字符串进行频繁的拼接，优先使用StringBuffer或StringBuilder类。

3. 在使用StringBuffer或StringBuilder时候最好能指定它们的容量。当不指定容量（capacity）时默认构造一个容量为16的对象。不指定容量会显著降低性能。

4. StringBuilder 一般使用在方法内部来完成类似 + 功能，因为是线程不安全的，所以用完以后可以丢弃。StringBuffer 主要用于多线程场景。
