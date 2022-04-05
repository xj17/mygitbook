1、Sting概述：字符串不可变，但是可以被共享，效果上相当于字符数组(char[]),底层原理是字节数组(byte[])

puublic final class String extends Object implements Comparable<String>...

2、String构造方法

3、String对象的特点

- 通过new创建的字符串对象，每一次new都会申请一个内存空间，内容相同，地址值不同。
- 以" "方式给出的字符串，只要字符序列相同，jvm只会建立一个String对象，并在字符串池中维护。

4、字符串的比较

- 基本类型：比较数据值
- 引用类型：比较地址值

5.String方法 

- charAt(int index); 返回指定索引处的值
- equals(Object object); 比较字符串是否相同
- length(); 返回此字符串的长度

**6.StringBuilder概述**

StringBuilder对象是一个可变的字符串类，可变指的是StringBuilder对象中的内容是可变的。

6.1 StringBuilder的添加和反转

- public StringBuilder append(任意类型);  //添加数据，并返回对象本身
- public StringBuilder  reverse()； //返回相反的字符序列
- public String toString(); //把StringBuilder 转换为String

7.String与StringBuilder相互转换

//StringBuilder sb=new StringBuilder ();

- String str=sb.toString();    //StringBuilder—>String
- StringBuilder sb=StringBuilder(str); //通过给构造方法把String转换为 StringBuilder 

