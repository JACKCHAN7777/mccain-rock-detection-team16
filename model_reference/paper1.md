一：What we learned from this paper：

1. 将石头检测问题定义为目标检测（Object Detection）问题，通过 bounding box + 分类完成任务  
2. YOLO 作为单阶段检测模型，具有速度快、适合实时检测（real-time）的优势  
3. 迁移学习（Transfer Learning）是关键，在小数据集上显著提升性能（mAP从18.2%提升到55.9%）  
4. 模型评估需要关注：  
   - mAP（准确率综合指标）  
   - FPS（推理速度）  
5. 存在明显的 accuracy vs speed trade-off：  
   - YOLO → 快  
   - Faster R-CNN → 更慢但结构更复杂 (s00603-025-04641-2.pdf)  

二：Models to consider：

1. YOLOv8（baseline），作为主要模型，适合实时检测和部署  
2. Faster R-CNN（精度对比模型），经典 two-stage 模型，用于对比 accuracy  
3. YOLOv8n / MobileNet-SSD（轻量模型），参数量小，适合 edge device（如 Raspberry Pi）  
4. YOLO + Attention，引入 CBAM attention 提升特征提取能力，在不增加太多计算成本下提高精度  

三：Experimental ideas：

1. 对比 YOLO vs Faster R-CNN（分析 accuracy 与 speed 差异）  
2. 对比 lightweight 模型 vs full 模型（如 YOLOv8 vs YOLOv8n / MobileNet）  
3. 评估 accuracy vs speed trade-off（mAP vs FPS）  
4. 测试迁移学习效果（pretrained vs 从零训练）  

Reference：

Yu, S., & Wong, L. N. Y. (2025)  
Att-YOLO: A Real-Time Rock Core Classification and Localization Deep Learning Model 
