# YOLOV3 Based Drone Detection System

**Requirements:**
- Ensure environment specifications in requirement.txt.
- Download pre-trained YOLOv3 weights.
- Download a test image of a dog.

**Implementation Steps:**
1. **Acquire Dataset:**
   - Obtain dataset 
   - Alternatively, create a custom dataset by collecting images and generating .xml files using LabelImg.

2. **Training:**
   - Configure paths in config.json for train and annotation folders.
   - Edit config.json to specify model details such as input size, anchors, and labels.
   - Generate anchors for the dataset using gen_anchors.py.
   - Commence training process using train.py.
   
3. **Detection:**
   - Utilize trained weights to detect drones in images, videos, or real-time feeds.
   - Execute prediction using predict.py, specifying the configuration file and input source (image, video, or webcam).

4. **Evaluation:**
   - Assess model performance by computing mAP on the validation dataset using evaluate.py.

**Output:**
- The system provides visualizations with detected bounding boxes on input images or videos.
