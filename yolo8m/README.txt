YOLOv8m-seg Complete Results
============================

Model:
YOLOv8m-seg

Training:
50 epochs
Image size: 512 x 512

Independent test set:
7 images captured with unseen background 9.

Inference settings:
Confidence threshold: 0.25
NMS IoU threshold: 0.7
Mask threshold: 0.5

Mean test results:
Dice: 0.865104
IoU: 0.803208
PSNR: 17.628 dB

Colour legend for overlays and error maps:
Green = true-positive foreground
Red = false-positive foreground
Blue = false-negative foreground
Black = correctly predicted background

Folder structure:
images/originals
images/ground_truth_masks
images/predicted_masks
images/probability_masks
images/overlays
images/error_maps
comparisons
metrics
training
model