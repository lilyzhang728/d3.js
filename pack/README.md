绘制打包图
====
打包图是干啥用的？一圈套一圈还挺好看的~<br>
实际上打包图是表示包含与被包含关系的一种图表，同时圈的大小也显示了各对象的权重<br>

好了说一下实现的要点吧<br>
- 首先是必须的步骤，转化数据，用的是 d3.layout.pack(),通过size()和radius()设置范围和最小半径<br>
- 读取数据用d3.json()<br><br>
其他的也没啥特别之处了==<br>


![](https://github.com/lilyzhang728/d3.js/blob/master/pack/img/demo.PNG)
