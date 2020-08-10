# DeepDreamStream
Attempt to create live stream of google's deep dream generator in a virtual ip webcam interface 
([Using Obs and NDI plugin](https://obsproject.com/forum/resources/obs-ndi-newtek-ndi%E2%84%A2-integration-into-obs-studio.528/))

Proccess goes like this:

Capture video through usb camera on client pc
Send footage via imagezmq to the server pc where each frame is beeing feeded to a pretrained deepdream caffe model (imagenet dataset)
and output the processed frame to a live stream (The two pcs are in the same LAN network) .

Resources/Credits:

https://opencv-python-tutroals.readthedocs.io/en/latest/py_tutorials/py_tutorials.html

https://www.pyimagesearch.com/2019/04/15/live-video-streaming-over-network-with-opencv-and-imagezmq/

https://github.com/google/deepdream

https://github.com/graphific/DeepDreamVideo

https://www.tensorflow.org/tutorials/generative/deepdream

https://medium.com/@ODSC/the-beginners-guide-for-video-processing-with-opencv-4e39795b942a




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

conda activate tf-gpu-cuda8
