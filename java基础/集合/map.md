Map集合—interface Map<K,V>

K:键的类型 V:值的类型； 

将键映射到值的对象；不能包含重复的键；每个键可以映射到最多一个值

一、HashMap

public class HashMap<K,V> extends AbstractMap<K,V> implements Map<K,V>...

重写了toString方法

V put (K key,V value); //将指定的值与该映射的指定键相关联 可以用来添加元素，键出现重复的，会将之前的覆盖。（HashMap—保证Map集合键的唯一性）

二、创建Map集合的对象

- 多态
- 具体的实现类HashMap

三、方法

- V remove(Object key);

- void clear();

- boolean containsKey(Object key);

- boolean containsValue(Object value);

- boolean isEmpty();

- int size();


**四、Map集合的获取功能**

- V get(Object key)；//根据键获取值
- Set <K> keySet(); //获取所有键的集合
- Collection <V> values; //获取所有值的集合
- Set <Map.Entry <K,V>> entrySet()l //获取所有键值对**对象**的集合

