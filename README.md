# removeWatermark
remove watermark from the image of antiquarian book  
輸入古籍之彩色影像，輸出去除浮水印之黑白影像

使用Otsu方法雖然能做到去除浮水印，但會有部分文字幾乎消失，如下圖。
![一般方法](/output1.jpg)

而使用本函式能在去除浮水印的同時也盡可能保留其他文字，如下圖。
![本方法](/output2.jpg)


#### 函式之參數說明
> removeWatermark(img, watermark_area)

    Args:
        img: Input img in grayscale. 2D numpy array.
        
        watermark_area: Topleft and bottomright of the watermark area. 
            For example: [(x1, y1), (x2, y2)]
            where (x1, y1) is topleft, (x2, y2) is bottomright. 
            Types of x1, x2, y1 and y2 are int.
    
    Return:
        img_result: A binary img without watermark.

#### usage
    img_result = removeWatermark(img, watermark_area)