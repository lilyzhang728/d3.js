制作中国地图
====
需要先用投影函数 d3.geo.mercator() 把geojson中的三维经纬度信息转换成二维的数据<br>
再使用地理路径生成器 d3.geo.path().projection()  根据刚才转成的二维数据生成 \<path> 元素的路径值 <br>
通过d3.json("china.geojson",function(){...}) 来读取数据，在svg画布上就可以画出经过一系列转化过后的地图啦~


![](https://github.com/lilyzhang728/d3.js/blob/master/geography/img/demo.PNG)
