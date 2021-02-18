# removeWatermark
remove watermark from the image of antiquarian book
輸入古籍之彩色影像，輸出去除浮水印之黑白影像

其中 watermark 為浮水印範圍，以左上角與右下角點座標 (x, y) 表示
topleft = (x1, y1)
bottomright = (x2, y2)
watermark = [topleft, bottomright]

inputfile 為輸入影像的檔案路徑+檔名
outputfile 為輸出影像的檔案路徑+檔名