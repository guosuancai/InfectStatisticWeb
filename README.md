# InfectStatisticWeb-221701338-221701338
  
# 一、作业链接  
|  这个作业属于哪个课程  |  [2020春W班](https://edu.cnblogs.com/campus/fzu/2020SpringW)  |
| :--: | :--: 
|这个作业要求在哪里|[作业要求](https://edu.cnblogs.com/campus/fzu/2020SpringW/homework/10456)|
|这个作业的目标|采用Web技术实现疫情统计的功能|
|作业正文|[结对第二次作业](https://www.cnblogs.com/suancai/p/12443657.html)|
|其他参考文献| csnd 博客园 github |  
# 二、结对学号  
- <font size="5">郭福强  221701338</font>  
链接：[](https://www.cnblogs.com/suancai/p/12443657.html)
- <font size="5">郭秋中  221701319</font>  
链接：[](https://www.cnblogs.com/QZcn/p/12465814.html)
  
# 三、项目介绍  
- **<font size="5">项目概括</font>**  
1. **要求**  
使用Web技术实现疫情统计可视化功能。
2. **实现**  
本次作业我们采用html+css+js来实现，用到了js的一些框架来实现地图功能。数据是采用静态存储的方式使用。    
- **<font size="5">具体功能</font>**   
1. **功能1：实现通过地图的形式来直观显示疫情的大致分布情况，还可以查看具体省份的疫情统计情况。**   
- 可以选择具体的日期
- 在全国地图上使用不同的颜色代表大概确诊人数区间
- 颜色的深浅表示疫情的严重程度，可以直观了解高危区域
- 鼠标移到每个省份会高亮显示
- 点击鼠标会显示该省具体疫情情况；
2. **功能2：点击某个省份显示该省疫情的具体情况**
- 可以选择具体的日期；
- 显示该省份对应的感染患者人数、疑似患者人数、治愈人数、死亡人数；
- 该省份到目前为止的新增确诊趋势、新增疑似趋势、治愈趋势和死亡趋势；
- 绘制该省份的趋势变化曲线图；
- **<font size="5">详细介绍</font>**  
1. **地图绘制:使用Echart**
- 导入echart.js和china.js两个js文件来进行绘制
- 先对获取地图需要放置的位置的元素,对该元素进行初始化。获取date控件中的日期，使用数组来获取每个地区的确诊人数。
- 设置地图的标题,设置省份和赋值。
- 设置点击地图和鼠标悬浮的事件。点击地图会跳转到相应地区的详细情况。鼠标悬浮位置会高亮显示，并显示该地区的确诊人数。
2. **选择时间的设置**
- 使用input标签中的date控件,通过选择时间来更改。
- 用element.value来访问时间。
- 确定时间后，点击某地区时也会将该时间和地区名传递给详细情况的页面。
3. **折线图绘制**
- 使用Echart进行绘制,可以根据当前日期获取过去一周的数据显示在折线图上。
- 绘制三个类型的折线图,可以更具按钮进行切换。 
4. **数据使用**
- 本次作业的数据采用静态数据形式，在开始作业之前使用第二次寒假作业做的程序处理数据，然后将处理好的数据
存储在数组里。
- 数组的形式为qz["北京2020-01-31"]，形如此类。qz代表确诊，数组名为数据的类型。  
# 如何运行  
1. 由于本次作业我们小组采用静态存储数据的方式，因此只有部分地区可以使用完整功能。
2. 完整功能的地区：安徽、北京、湖北、福建、浙江
3. 完整功能的日期：2020-01-25、2020-02-02  
