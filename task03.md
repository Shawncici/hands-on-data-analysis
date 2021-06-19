![image](https://user-images.githubusercontent.com/33819026/122631006-bdd22780-d0fa-11eb-9612-4a26ee3bfa11.png)
### 数据合并
pandas的concat函数最好用，可以左右或上下拼接，调整axis即可，1位左右，0为上下。

groupby 的用法如图有两种表达方法，第一种前后都要写“text”，第二种只用在前边写“text”。
groupby两个参数的结果如第三个代码块所示
![image](https://user-images.githubusercontent.com/33819026/122631025-dcd0b980-d0fa-11eb-9c02-a25ad0ea5a2c.png)


### pandas中很多函数（比如concat都有axis这个参数，它的不同取值分别是什么含义？参数的默认取值是什么？
axis参数是指延行或列方向进行某个操作，0代表行方向（纵向），1代表列方向（横向），默认为0（纵向）

### 对数据groupby后常用的聚合函数有哪些？如何实现对不同的列采取不同的聚合函数？
常用聚合函数：mean/sum/size/count/std/var/sem/describe/first/last/nth/min/max
