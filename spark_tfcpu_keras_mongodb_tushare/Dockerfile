FROM tensorflow/tensorflow:latest-py3-jupyter
RUN pip install pandas numpy keras pymongo tushare pyspark
ENV mongohost "172.17.0.1"
ENV PYTHONPATH=".:${PYTHONPATH}"
WORKDIR "/app"
CMD ["bash", "-c", "source /etc/bash.bashrc && jupyter notebook --notebook-dir=/app --ip 0.0.0.0 --no-browser --allow-root"]