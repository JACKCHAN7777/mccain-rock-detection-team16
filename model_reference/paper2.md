一：What we learned from this paper：（MobileNet-SSD）



1.将目标检测应用于视频流（video stream），实现实时目标检测（real-time object detection） (3379247.3379264.pdf)


2.采用 MobileNet + SSD（Single Shot Detector）组合，实现高效目标检测模型 (3379247.3379264.pdf)


3.MobileNet 作为 backbone，可显著减少参数量和计算复杂度，适合嵌入式设备（embedded systems） (3379247.3379264.pdf)


4.SSD 作为单阶段检测器，可同时完成定位（localization）和分类（classification），提升检测速度 (3379247.3379264.pdf)


5.预训练模型（pre-trained model）可直接用于多类别目标检测，无需从零训练 (3379247.3379264.pdf)


6.模型在实验中可达到约 14 FPS，满足实时检测需求 (3379247.3379264.pdf)


7.存在明显的 accuracy vs speed trade-off：

R-CNN 系列 → 精度高但计算复杂

MobileNet-SSD → 更轻量、更快但精度略低 (3379247.3379264.pdf)





二：Models to consider：



1.MobileNet-SSD（轻量模型），结合 MobileNet backbone 与 SSD 检测器，适合实时检测与 edge device 部署


2.YOLOv8（baseline），作为主要模型，适合实时检测和部署


3.YOLOv8n（轻量模型），相比 YOLOv8 更小、更快，适合嵌入式设备


4.Faster R-CNN（精度对比模型），经典 two-stage 模型，用于对比 accuracy



三：Experimental ideas：



1.对比 MobileNet-SSD vs YOLOv8（轻量模型 vs 高性能模型）


2.对比 MobileNet-SSD vs YOLOv8n（不同轻量模型）


3.评估 accuracy vs speed trade-off（mAP vs FPS）


4.测试预训练模型效果（pretrained vs 从零训练）



Reference：

Younis, A., Li, S., Shelembi, J. N., & Zhang, H. (2020)

Real-Time Object Detection Using Pre-Trained Deep Learning Models MobileNet-SSD
