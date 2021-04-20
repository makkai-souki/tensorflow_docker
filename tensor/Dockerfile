FROM tensorflow/tensorflow:latest-gpu-py3-jupyter

RUN apt-get update
RUN apt-get install -y libfreetype6-dev libxft-dev python-opengl
RUN apt-get install -y x11-apps

RUN pip install --upgrade pip

RUN pip uninstall tensorflow
RUN pip install tensorflow==2.1.0
RUN pip install google_images_download
RUN pip install matplotlib
RUN pip install pillow
RUN pip install keras
RUN pip install tensorflow-hub
RUN pip install six
RUN pip install scikit-image
RUN pip install keras-rl2
RUN pip install gym

ENV NVIDIA_VISIBLE_DEVICES all
ENV NVIDIA_DRIVER_CAPABILITIES utility,compute