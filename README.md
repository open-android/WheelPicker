# 最火Android开源项目WheelPicker使用
---
开源地址：[https://github.com/open-android/WheelPicker](https://github.com/open-android/WheelPicker "开源项目地址")

 PS：如果觉得文章太长，你也可观看该课程的[视频](https://www.boxuegu.com/web/html/video.html?courseId=172&sectionId=8a2c9bed5a3a4c7e015a3bbffc6107ed&chapterId=8a2c9bed5a3a4c7e015a3adeb65b03f1&vId=8a2c9bed5a3a4c7e015a3ab4fe0601bb&videoId=F94BC8E95143C10D9C33DC5901307461)，亲，里面还有高清，无码的福利喔

# 运行效果

![](http://i.imgur.com/TPkIrBJ.gif)

* 爱生活,爱学习,更爱做代码的搬运工,分类查找更方便请下载黑马助手app


![黑马助手.png](http://upload-images.jianshu.io/upload_images/4037105-f777f1214328dcc4.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

## 使用步骤

### 1. 在project的build.gradle添加如下代码(如下图)

	allprojects {
	    repositories {
	        ...
	        maven { url "https://jitpack.io" }
	    }
	}

![](http://oi5nqn6ce.bkt.clouddn.com/itheima/booster/code/jitpack.png)


### 2. 在Module的build.gradle添加依赖

     compile 'com.github.open-android:WheelPicker:v1.0.0'


### 3. 复制如下代码到xml

    <com.itheima.wheelpicker.WheelPicker
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        app:wheel_atmospheric="true"
        app:wheel_curved="true"
        app:wheel_cyclic="true"
        app:wheel_selected_item_position="5"
        app:wheel_item_text_color="#66ff0000"
		app:wheel_selected_item_text_color="#6600ffff"/>


    <!--属性解释:
	
        wheel_atmospheric :  条目颜色是否执行衔接处理 效果更好
        wheel_curved ： 是否是弧形状态显示
        wheel_cyclic : 是否可循环
        wheel_selected_item_position ： 默认选中第几个条目
        wheel_item_text_color 未选中的条目颜色
        wheel_selected_item_text_color  选中的条目颜色-->

###4 . 运行即可

#### 细节注意:

> 默认会自带一组数据，所以无需设置数据。 若想设置新的数据，可通过 调用如下方法即可

		setData(List data); 

* 详细的使用方法在DEMO里面都演示啦,如果你觉得这个库还不错,请赏我一颗star吧~~~

* 欢迎关注微信公众号

![](http://oi5nqn6ce.bkt.clouddn.com/itheima/booster/code/qrcode.png)
