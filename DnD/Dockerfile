FROM ubuntu:20.04

WORKDIR /home
RUN apt update
RUN DEBIAN_FRONTEND=noninteractive apt install -y python3 python3-pip libboost-python-dev libboost-numpy-dev libcpprest-dev wget
RUN wget -q https://github.com/microsoft/onnxruntime/releases/download/v1.10.0/onnxruntime-linux-x64-1.10.0.tgz
RUN tar -zxf onnxruntime-linux-x64-1.10.0.tgz --strip-components=2 -C /usr/local/lib --wildcards "*/lib/lib*"
RUN rm onnxruntime-linux-x64-1.10.0.tgz
RUN pip config set global.index-url https://mirrors.aliyun.com/pypi/simple && \
    pip config set install.trusted-host mirrors.aliyun.com && \
    pip3 install numpy==1.24.3 pyelftools pefile yapf argparse onnx tensorflow tensorflow tf2onnx
COPY ./ .
RUN wget -q https://raw.githubusercontent.com/onnx/tensorflow-onnx/main/tools/dscripts/dump-onnx.py -O scripts/dump-onnx.py
CMD ["bash"]
