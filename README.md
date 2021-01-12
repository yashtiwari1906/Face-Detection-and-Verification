# Face-Detection-and-Verification
In this we are using S3FD for detection of faces and inception resnet v1 for generating a 512 dimensional embedding which will be further used for verification.
Here we are taking a small video clip from the TV series named Big Bang Theory in which we are trying to locate seven of its characters namely- Sheldon, Leonard, Howard, Raj, Penny, Amy, Bernadette, Emily and Stuart. If any of the other face will come in detection it will be simply shown by the unknown.
One example for detection is shown below-

![alt text](https://github.com/yashtiwari1906/Face-Detection-and-Verification/blob/master/Images/BBT_cast_image.jpg)

# Procedure
- First decide the number of characters to be detected in a frame and try to get one-one photo of those characters.
- Firstly prepare a database in which embedding vector of these characters will be there and decide a threshold value
- Now start processing the video frame by frame, now in a frame the detector will try to find the different peoples in that frame and then each face will be passed through           recognizer and an embedding vector will be generated which will be compared with all the embedding vectors in our database whichever have smallest cosine distance and the value   of that distance should be less than some threshold that image's name will be put forward on the bounding box of that face.
- Likewise all the faces in the frame will follow the above process.

# Drive link
https://drive.google.com/drive/folders/1iVJnedI2jVJxXmJWCDOtSB9J95RwJ5e4?usp=sharing
In above link all the required images, weights and videos are there which are used in this project.

# Refferences
- https://github.com/shaoanlu/face_toolbox_keras
- https://openaccess.thecvf.com/content_ICCV_2017/papers/Zhang_S3FD_Single_Shot_ICCV_2017_paper.pdf
- https://arxiv.org/pdf/1602.07261.pdf
- https://github.com/somasundaram1702/Unknown-face-recognition



