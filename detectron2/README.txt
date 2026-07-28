DETECTRON2 MASK R-CNN R50-FPN RESULTS
=====================================

Model:
Mask R-CNN with ResNet-50 and FPN

Framework:
Detectron2

Training:
- Training images: 49
- Validation images: 7
- Test images: 7
- Epoch equivalent: 50
- Input resolution: 512 x 512
- Pretraining: COCO
- Score threshold: 0.25

Independent test results:
- Mean Dice: 0.732977
- Dice standard deviation: 0.271097
- Mean IoU: 0.635542
- IoU standard deviation: 0.269595
- Mean PSNR: 13.889 dB
- PSNR standard deviation: 2.424 dB
- Mean precision: 0.714886
- Mean recall: 0.780389
- Mean pixel accuracy: 0.952621
- Mean inference time: 126.195 ms/image
- Throughput: 7.92 images/second

Error-map colours:
- White: true positive
- Red: false positive
- Blue: false negative
- Black: true negative

Important:
All predicted Detectron2 instances were merged into one binary
foreground mask before calculating Dice, IoU, and PSNR.