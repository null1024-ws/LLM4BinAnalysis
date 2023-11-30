FROM ubuntu:20.04

WORKDIR /home
RUN apt update
RUN DEBIAN_FRONTEND=noninteractive apt install -y python3 python3-pip libboost-python-dev libboost-numpy-dev libcpprest-dev wget
RUN wget -q https://repo.anaconda.com/archive/Anaconda3-2023.09-0-Linux-x86_64.sh && sh Anaconda3-2023.09-0-Linux-x86_64.sh -b -p /usr/local/anaconda3
RUN export PATH=$PATH:/usr/local/anaconda3/bin && conda create -n xda python=3.7 numpy scipy scikit-learn colorama && conda init bash && conda activate xda
RUN echo "source /root/.bashrc && conda activate xda ; conda install -y pytorch torchvision torchaudio cudatoolkit=11.0 -c pytorch ; pip install --editable ." > start.sh
COPY ./ .
CMD ["bash"]

