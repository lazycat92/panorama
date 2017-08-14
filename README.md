# 基于[Panolens.js](https://pchen66.github.io/Panolens/)和[Three.js](https://github.com/mrdoob/three.js/)

#### 做全景图用Panolens.js

[demo](https://lazycat92.github.io/panorama/index)

##### 效果图
![动态图片](https://github.com/lazycat92/panorama/blob/master/panorama.gif)

#### 用法(Usage)

```
<script src="js/three.min.js" type="text/javascript" charset="utf-8"></script>
<script src="js/panolens-offline.min.js" type="text/javascript" charset="utf-8"></script>
```

先引入相关的js文件，然后初始化全景图

```
<script>

    var panorama, viewer;

    // 选择全景图照片
    panorama = new PANOLENS.ImagePanorama( 'asset/equirectangular.jpg' );  

    // 创建全景图容器
    viewer = new PANOLENS.Viewer();
    
    // 将全景图添加到容器中
    viewer.add( panorama );

</script>
```
若是没有定义全景图容器，那么容器会默认为body。
