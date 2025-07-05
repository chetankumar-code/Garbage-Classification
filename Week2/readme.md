
In the week 2 , several updates to the original garbage classification code is being done to improve the test as well the training accuracy .
Optimization of the code is done on the several key areas including the:

Better Input Resolution: We updated the image input size to 260x260 to match the default input resolution of EfficientNetV2B2. This helps the model retain more features and improves classification accuracy.

Efficient Preprocessing: Introduced preprocess_input from the EfficientNet API to ensure images are normalized correctly before feeding into the model.

Faster Data Loading: We enabled TensorFlow’s cache() and prefetch() pipelines on all datasets. This reduces I/O bottlenecks and accelerates training.

Improvement in the data augmentation my changing or updating the values of the rotation and the updation and use of the TTA i.e the Test time augmentation and the evaluation with the test time augmentation.
