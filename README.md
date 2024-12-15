# underwater-plastic-pollution-computer-vision

## Leveraging ML to scale Plastic Pollution Cleanup in Water Bodies

This study will focus on how Machine Learning technology can be used to help in detecting plastic in water bodies using satellite and drone images, so that cleanup efforts are deployed in right location with right resources.

*Object detection* is a deep learning approach which localizes and simultaneously classify different objects present in a digital image. Object detection technique draws bounding boxes on the objects and also categorize the class of such objects at the same time. Object detection technique will best suitable for this study because the goal is to identify the exact location of plastic waste only if present in digital images.

### Datasets

The dataset identified for this study is taken from [Data Repository][1] for the University of Minnesota (DRUM).  The dataset contains images of various different kinds of marine debris that are captured from real underwater environments where the objects are in different states of decay, occlusion, and overgrowth. The images are labeled with bounding boxes on instances of trash, biological objects such as plants and animals, and ROVs (Fulton et al., 2020).

[1]:https://conservancy.umn.edu/handle/11299/214366


### Approach
YOLO (You Only Look Once) is a state-of-the-art, real-time object detection deep learning architecture in which a single convolutional network detects the bounding boxes and class probabilities of these boxes. It divides image into grid of cells and the network predicts the class probability, bounding boxes and confidence score for each cell. Then Non-max Suppression filtering algorithm is used to select only relevant probabilities to finalize the class or classes based on confidence threshold. 

![YOLO Object detection](./img/yolo_process.png)