# AI4ALL_ASL_AI
---
### MediaPipe.ipynb
#### Phase 1:
- initially used resnet-50 to transfer learn ASL alphabet using 1200 collected image per alphabet
- Peak accuracy: 77% (low accuracy is likely due to complexity/lack of localization of hand as it takes input of whole image.
#### Phase 2:
- Instead used Mediapipe to extract 63 points (21 points of x, y, z of a hand joints)
- Then used Multi-layer perceptron to classify
- Peak accuracy 98.2%, performed very good even in low quality camera as it only need 63 point from mediapipe to be properly given.
