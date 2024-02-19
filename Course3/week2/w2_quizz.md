# Object Detection Quiz Notes
1. **Improving Object Detection Accuracy**
    - Techniques that can be used include:
        - Scaling down the image and then detecting the object within it using the bounding box.
        - Using the Selective Search technique.
        - Increasing the size of the bounding box until the object fits entirely in it.

2. **Selective Search Insights**
    - True statements:
        - It identifies larger objects by grouping together initially identified smaller objects.
        - Image segmentation is used in this technique to identify smaller objects.
    - Incorrect statement:
        - The biggest bounding box detected of the smaller objects in the end becomes the final bounding box around the identified object. (This statement should not have been selected.)

3. **Non-Maximum Suppression (NMS)**
    - The technique of selecting the best bounding box based on the highest IoU between the true label and several predicted bounding boxes is called non-maximum suppression.

4. **NMS Technique Application**
    - For an image with multiple colored bounding boxes around a football, the correct bounding box selected according to the NMS technique would be the one that encapsulates the maximum area of the object.

5. **R-CNN vs. Fast R-CNN**
    - A difference between R-CNN and Fast R-CNN is that Fast R-CNN does not generate regions of interest; instead, it expects them as input, contrary to R-CNN, which generates regions of interest from the input image.

6. **Code Analysis**
    - True statements about the provided code snippet include:
        - `label_id_offset` is an adjustment for any offset between the ‘detection classes’ starting index and the actual starting index.
        - `min_score_thresh` is used to exclude object labels and their bounding boxes if their score is below the set threshold.
    - Incorrect statement:
        - Setting `use_normalized_coordinates=True` indicates that bounding box coordinates are already normalized.

7. **Model Initialization and Pre-trained Weights**
    - The statement regarding the code initializing a model and restoring pre-trained weights using the .config file method was incorrectly marked as true.

8. **Printing Trainable Variables**
    - The correct syntax to print a list of trainable variables in a model is:
        ```python
        for varName in myModel.trainable_variables:
            print(varName.name)
        ```
