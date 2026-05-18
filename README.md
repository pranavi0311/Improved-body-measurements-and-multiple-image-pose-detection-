# Improved-body-measurements-and-multiple-image-pose-detection

*Task 1: Improve Body Measurement Accuracy*

Body measurement gets wrong because:
1. *No scale* – Camera doesn’t know if person is close or far. Fix: put a reference like A4 paper in frame, or ask for user’s height.
2. *Shaky keypoints* – Pose model jumps a bit. Fix: average keypoints over 5 frames to smooth it.
3. *Wrong angle* – Side view makes arms look shorter. Fix: only measure when person faces camera straight.
4. *Loose clothes* – Hides body. Fix: use cloth segmentation to see body shape under clothes.

*Task 2: Test Pose Detection on Multiple Images/Videos*

You’re checking if pose detection works in different cases:
- Different poses: T-pose, side, sitting
- Different light: dark, bright, backlight  
- Different clothes: tight, loose, patterns
- Different distance: close, far
