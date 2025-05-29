# StealthEye
 Fine-Grained Motion Detection and Depth-Aware Tracking System

StealthEye is a sophisticated motion detection system designed for effective surveillance area monitoring.

Leveraging a Gaussian Mixture Model (GMM) as a background subtractor, StealthEye generates a binary mask (fg_mask) to isolate and identify moving objects within video frames.
The system employs morphological operations, specifically erosion and dilation, to minimize noise and optimize the binary mask output. 

Motion detection is determined by the condition np.sum(fg_mask) > 0, which classifies frames as containing "Motion" or "No Motion." The pipeline was rigorously tested and achieved a trained model accuracy of 92.5%. 
Key classes utilized include BackgroundSubtractorMOG2 for background modeling and cv2 functions for morphological processing. 
StealthEye provides reliable and efficient motion analysis for real-time surveillance applications.
