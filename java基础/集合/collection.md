1、集合

- Collection—单列（List—可重复（Arraylist、LinkedList...）、Set—不可重复(HashSet、TreeSet...)
- Map—双列

2、Collection是单列集合的顶层接口，它表示一组对象

public **interface** Collection<E>

3、创建Collection集合的对象

- 多态
- 具体实现类ArrayList  //Collection<String>c=new ArrayList<>();

4.常用方法

add、remove、clear、contains、isEmpty、size

5.遍历

**interface** Iterator<E> ——迭代器、集合的专用遍历方式

- E：next();
- boolean hasNext();

