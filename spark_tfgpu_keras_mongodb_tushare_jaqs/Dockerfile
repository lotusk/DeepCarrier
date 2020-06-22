FROM tensorflow/tensorflow:latest-gpu-py3-jupyter
RUN apt-get install -y libsnappy-dev
RUN pip install pandas numpy keras pymongo tushare pyspark python-snappy jaqs
ENV mongohost "172.17.0.1"
ENV PYTHONPATH=".:${PYTHONPATH}"
WORKDIR "/app"
CMD ["bash", "-c", "source /etc/bash.bashrc && jupyter notebook --notebook-dir=/app --ip 0.0.0.0 --no-browser --allow-root"]
