<<<<<<< HEAD
# 外部JavaScript 加载方式比较
###1.  append head 方式, 动态在head部分增加script节点

异步方式加载,执行顺序为

1. js1 appendChild Start
2. js1 appendChild Finish
3. js2 execute finish
4. js1 execute finish

第二段js执行完后,再执行第一段,无法保证执行顺序与载入顺序一致.

###2. document.write方式,动态输出script语句

同步方式加载,执行顺序为

1. js1 write start
2. js1 write finish
3. js1 execute finish
4. js2 execute finish

执行顺序与载入顺序保持一致.

=======
append head
异步方式加载,执行顺序为
js1 appendChild Start
js1 appendChild Finish
js2 execute finish
js1 execute finish
>>>>>>> FETCH_HEAD
