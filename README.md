
Run checkout_detector.py to test the model on video_test.avi. Now it is configured to run on CPU. Please change the config parameters to run on GPU.

This will create a new file output.avi with all detections.

Model Details:

==>For this task, i have used a pretrained SSD model with inceptionv2, and finetuned it to out target dataset. Since this is going to be a real time object detection we cannot comprimise on speed. As there is a trade off between speed and accuracy, we have to select the model depending up on our requirement. SSD is one of the best object detection architecture and is well known for its speed without trading much on the accuracy. This is the reason i went for a SSD architecture than a RCNN based model. 

==>Python script for evaluating the model on test video, is multithreaded so that the speed with which frames are processed is much better than original.


