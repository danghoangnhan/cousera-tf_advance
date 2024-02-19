# Introduction and Concepts of Computer Vision Quiz Notes

## Week 1

### Questions and Answers

1. **Multi-Class vs. Multi-Label Classification**
    - **Question**: In a Multi-Class classification scenario, can your model identify all the different items and people that are present in a given input image?
    - **Answer**: True. This statement is correct for Multi-Label classification.
  
2. **Object Detection vs. Object Localization**
    - **Question**: Which statement correctly describes the difference between object detection and object localization?
    - **Answer**: Incorrectly answered in quiz. The correct distinction involves object detection identifying multiple objects within an image and object localization identifying the location of a single main subject.
  
3. **Semantic Segmentation**
    - **Question**: What is the method that locates an object(s) by labeling the pixels, where each similar object(s) is assigned to the same class?
    - **Answer**: Incorrect spelling of "image segmentation" was marked. The intended answer seems to be "semantic segmentation."
  
4. **Transfer Learning**
    - **Question**: In the context of Transfer Learning, what is the initial training task where the model learns reusable patterns called?
    - **Answer**: False. It is called a pre-training task.
  
5. **Benefits of Transfer Learning**
    - **Question**: Check all the scenarios in which Transfer Learning could be beneficial.
    - **Answers**: 
        - To reduce computation and processing cost
        - When the task is a sub-task of an already trained, larger model
        - When there's insufficient data for the task, resembling another already trained task
        - To ensure better performance
  
6. **Upscaling Images with TensorFlow**
    - **Question**: What is the name of the built-in TensorFlow layer-type which you can use to increase the dimensions of a 2D image?
    - **Answer**: UpSampling2D.
  
7. **Upscaling Dimensions**
    - **Question**: You have an image of dimensions 48 x 48, and you want to upscale it to 240 x 240 using UpSampling2D. What size do you pass in?
    - **Answer**: (5, 5).
  
8. **Understanding `include_top=False`**
    - **Question**: What does “include_top=False” mean?
    - **Answer**: It discards the top most layers of ResNet50 when initializing my_layer using ResNet50.
  
9. **Bounding Box Prediction Technique**
    - **Question**: What is the name of the technique used in the output dense layer that is used to predict Bounding Boxes?
    - **Answer**: Regression.
  
10. **Intersection Over Union (IoU)**
    - **Question**: Check all statements that are true regarding IoU, with regards to Bounding Boxes.
    - **Answers**:
        - The closer the value of IoU is to 0 the poorer is the prediction of the bounding box.
        - IoU is the area of intersection of the two boxes (true and predicted) divided by the total union area of the two boxes.