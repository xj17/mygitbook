set集合—public **interface** set<E> extends Collection<E>

1、set集合特点：不重复、没有带索引的方法，不能使用普通for循环遍历

2、哈希值：jdk根据对象的地址或字符串或数字算出来的int类型的数值

public int hashCode(); //返回对象的哈希码值，默认情况下，不同对象的哈希值不同。可以通过方法重写让不同对象的哈希值相同。

3、HashSet—public class **HashSet**<E> extends AbstractSet<E> implements  set<E>....

3.1HashSet集合特点

- 底层数据结构是哈希表
- 对集合的迭代顺序不作任何保证，意为不保证存储和取出的元素顺序一致
- 没有带索引的方法，不能使用普通for循环遍历
- 不重复


4、**哈希表**

jdk8之前，底层采用数组+链表实现，是一个元素为链表的数组

jdk之后，当长度比较长时，底层实现了优化

5、LinkedHashSet—class LinkedHashSet<E> extends HashSet<E> implements Set<E>...

LinkedHashSet集合是哈希表（唯一）和链表（有序、存取顺序一致）实现的set接口，具有可预测的迭代顺序

6、TreeSet—Class TreeSet<E>  extends AbstractSet<E> implements **NavigableSet**<E>...

NavigableSet—SortedSet—Set—间接实现set接口

6.1 自然排序Interface Comparable<T> 

无参构造方法，使用自然排序对元素进行排序的

自然排序是让元素所属的类实现Comparable接口，重写compareTo方法，注意要按照要求的主要条件和次要条件来重写。

6.2 比较器排序Interface Comparator<T>

带参构造方法，使用比较器排序对元素进行排序的

比较器排序是让集合构造方法接收Comparator的实现类方法，重写compare(o1,o2)方法





