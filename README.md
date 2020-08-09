# DeepDreamStream
Attempt to create live stream of google's deep dream generator in a virtual ip webcam interface (Linux?)

Resources:

https://opencv-python-tutroals.readthedocs.io/en/latest/py_tutorials/py_tutorials.html

https://github.com/gebart/python-v4l2capture
https://github.com/umlaeute/v4l2loopback
https://github.com/TimSC/libvideolive
https://github.com/google/deepdream
https://github.com/graphific/DeepDreamVideo
https://medium.com/@ODSC/the-beginners-guide-for-video-processing-with-opencv-4e39795b942a
https://www.youtube.com/watch?v=K_am9oMeweA


Prerequisites(Windows):

Install Anaconda3 and use Anaconda Powershell Prompt (Anaconda3)

conda create --name py35 python=3.5

conda activate py35

pip install imutils

pip install numpy

pip install imagezmq

pip install opencv-contrib-python

conda install -c conda-forge jupyterlab

conda install matplotlib

conda create -n tf-gpu tensorflow-gpu==2.0

conda activate tf-gpu

conda create -n tf-gpu-cuda8 tensorflow-gpu cudatoolkit=10.0
