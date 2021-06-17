## 缺失值观察与处理
df.isnull() ——判断数据是否为空值；

df.drop() —— 将某些列的数据隐藏

df.drop_duplicates() ——将对行有缺失值清理

![image](https://user-images.githubusercontent.com/33819026/122409671-e56ba780-cfb5-11eb-8071-a0e03943cdf7.png)

fillna：
value scalar, dict, Series, or DataFrame：缺失值的填充值
method{‘backfill’, ‘bfill’, ‘pad’, ‘ffill’, None}, default None：填充方法，前两个根据后面一个有效值填充，‘pad’、‘ffill’根据前一个有效值填充。
axis{0 or ‘index’, 1 or ‘columns’}：延行（列）方向填充。
inplace bool, default False：是否原地删除
limit int, default None：如果指定了方法，则这是要向前/向后填充的连续NaN值的最大数目。换句话说，如果与超过这个数目的连续的Nans有一个差距，它将只会被部分填补。如果未指定方法，则这是将填充NAN的整个轴上的最大条目数。如果不是零，则必须大于0。
downcast dict, default is None：填充缺失值后是否改变某列的Dtype，可以看下面示例。

dropna:
axis{0 or ‘index’, 1 or ‘columns’}, default 0：删除包含缺失值的行（列）
how{‘any’, ‘all’}, default ‘any’：所有都是na才删除，还是只要有一个na就删除
thresh int, optional ：删除到至少有多少na剩余
subset array-like, optional：针对某几列删除删除缺失值
inplace bool, default False：是否原地删除
