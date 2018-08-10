原因是对各种图片类型进行了指定的变换（如颜色通道、像素密度等），导致图片属性改变

void javax.imageio.ImageReader.setInput(Object input, boolean seekForwardOnly, boolean ignoreMetadata)

```
ImageIO.java

//第三个参数为true，表示不读取源图片的元数据（属性）
reader.setInput(stream, true, true);
```

1. jpg   变小  
![](http://onmer39jj.bkt.clouddn.com/18-8-10/65993824.jpg)

2.png   变大  
![](http://onmer39jj.bkt.clouddn.com/18-8-10/25904670.jpg)
