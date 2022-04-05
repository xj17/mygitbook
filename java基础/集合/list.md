List集合——public **interface** list<E> extends Collection<E>

**1、有序(存储和取出的元素顺序一致)、可重复**

2、方法

- public void add(E e); //将指定元素添加到此集合的末尾
- public void add (int index,E element);//在此集合的指定位置插入指定元素
- public boolean remove; //删除指定的元素
- public E remove(int index);
- public E set(int index,E element);
- public E get(int index);
- public int size();

3、并发修改异常

迭代器在遍历的过程中，通过集合对象修改了集合中元素的长度，造成了迭代器获取元素中判断预期修改值和实际修改值不一致

4.**Interface** ListIterator<E> extends Iterator<E>——列表迭代器

允许向任意方向遍历列表，在迭代期间修改列表，并获取列表中迭代器的当前位置

4.1 **ListIterator**中常用方法

- E next();
- boolean hasNext();
- E previous();
- boolean hasPrevious();
- void add(E e);


5.增强型for语句：简化数组和Collection集合的遍历

- 实现Iterator接口的类允许其对象成为增强型for语句的目标
- 内部原理——Iterator迭代器

//for(元素数据类型 变量名:数组或Collection集合){ }

6.数据结构

- 栈—先进后出—杯子—压/进栈、弹/出栈
- 队列—先进先出—排队
- 数组—查询快，增删慢
- 链表—增删快，查询慢

7.list集合子类

public class **ArrayList**<E> extends AbstractList<E>  implements List<E>...

- ArrayList—可调整大小的数组实现

public class **LinkedList**<E> extends AbstractSequentialList<E>  implements List<E>、Deque<E>...

- LinkedList—链表实现list接口

8.LinkedList 特有方法

- public void addFirst(E e);
- public vod addLast(E e );
- public E getFirst();
- public E getLast();
- public E removeFirst();
- public E removeLast();

