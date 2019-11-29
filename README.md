# lipColorDetector
本项目用于实现简单的人脸口红色号识别

运行  python detectmouth.py

具体逻辑：
1）先用dlib+opencv识别人脸和嘴唇
2）提取嘴唇区域色差较小的色块，求出平均RGB值
3）遍历存储好的口红品牌和型号仓库，用已有色块RGB值与库中口红RGB值对比，求最接近的数值
