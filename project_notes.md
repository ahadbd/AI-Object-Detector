# Project Notes: AI Object Detector

## Part 2: The Logic (Critical Thinking)

**1. Why is this "Supervised Learning"? (Hint: Did you provide the names for the objects?)**
This is considered "Supervised Learning" because we provided the computer with *labeled data*. By explicitly creating classes (categories) and providing the names for the objects (e.g., "Phone", "Calculator") along with the example images, we "supervised" the training process. The model learned to map the input images to the specific labels we provided.

**2. Edge Cases: What happens if you hold two objects at once? How does the computer react?**
If you hold two objects at once, the model will likely get confused and struggle to make a confident prediction. Since the model was only trained on images containing a single object at a time, seeing both sets of features in one frame will cause the confidence scores to split (e.g., jumping between 50% for one object and 50% for the other), or it might rapidly flicker back and forth between the two classifications as it tries to decide which defining features are more prominent.
