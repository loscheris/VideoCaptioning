# VideoCaptioning

Dependencies: OpenCV 3.2, Tensorflow 1.2, Caffe, skimage, pandas, numpy

1. Download and untar MSVD dataset from: http://www.cs.utexas.edu/users/ml/clamp/videoDescription/YouTubeClips.tar
3. Change the paths in cnn_util.py and extract_RGB_feats.py
4. Extract and save VGG16 features for ALL MSVD videos by running: python extract_RGB_feats.py
5. Split all these features into two different directories: 'training' and 'test' (I use 300 of them as test set)
6. Change the global parameters (paths to 'training' and 'test' directories) and training parameters (optional) in model_RGB.py
7. Train the model by running：python main.py
8. Test and evaluate the model by running: test() in model_RGB.py
