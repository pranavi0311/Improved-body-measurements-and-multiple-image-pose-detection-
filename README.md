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

<img width="820" height="712" alt="IMG_20260518_150200" src="https://github.com/user-attachments/assets/a35a0a3b-abba-43ca-bfeb-0b242050fe2e" />
<img width="800" height="1080" alt="IMG_20260518_150224" src="https://github.com/user-attachments/assets/6d0da821-8840-4684-9496-a07834a4625d" />
<img width="3168" height="1880" alt="IMG_20260518_151004" src="https://github.com/user-attachments/assets/de17eeb0-5eaf-43c7-b933-2f43a63be915" />
