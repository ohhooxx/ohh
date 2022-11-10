# ohh
```java
使用treeMap 作为概率和奖励对象的存储工具 【key-计算后的概率，value-奖励对象】
Random r =new Random();
设置一个概率最大倍数，multiple=100000
循环奖励list
Map map= new TreeMap();
for(int i=0;i<list.szie();i++){
  p=list.get(i);
  maxProbabilty += p.probability*multiple
  map.put(maxProbabilty,p);
}
rv=r.nextInt(multiple)+1;
map1=map.tailMap(rv);
if(map1.isempty){
递归抽奖
}else{
map1.firstKey();
}
```
