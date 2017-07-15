绘制集群图
====
集群图是另一种表示包含与被包含关系的图表，但是不能显示各对象的权重，个人觉得比较适合需要分类的对象比较多的情况，像中国省市地区县这样的，如果绘制打包图会非常庞大而且从属关系也不如集群图这样一目了然。

实现要点：  
转换数据用的是 d3.layout.cluster(), 也是用size 设置范围。  
因为需要绘制连线，因为是要绘制大括号，这里使用的是对角线生成器：d3.svg.diagonal(),只需要输入两个点的坐标，即可获得一条贝塞尔曲线！  
此处又使用了 projection(function(d) { return [d.y, d.x]; }); 使整个图横向显示

读数据用d3.json()



![](https://github.com/lilyzhang728/d3.js/blob/master/cluster/img/demo.PNG)
