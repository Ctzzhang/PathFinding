# 寻路算法整理，自己使用java实现完整代码及性能测试
## 主要整理格子地图的寻路算法，包括主流的A*和JPS及JPS+
### 测试地图数据使用项目中maps/maze-100-1.map
### 性能测试结果

#### A*寻路
 * 性能测试：

| 左对齐标题 | 右对齐标题 | 居中对齐标题 |
| :------| ------: | :------: |
| 短文本 | 中等文本 | 稍微长一点的文本 |
| 稍微长一点的文本 | 短文本 | 中等文本 |
 *  	次数	距离公式	启发函数	耗时ms	close大小		备注
 * 		10000	直接获得	manhattan	6000	1641		[1,39]->[99,65] 大概纵100*横25的距离，地形非常复杂，寻路节点80个。

#### JPS寻路
 * 性能测试：
 *  	次数	距离公式	启发函数	耗时ms	close大小		备注
 * 		10000	octile		manhattan	1600	419			[1,39]->[99,65] 大概纵100*横25的距离，地形非常复杂，寻路节点80个。