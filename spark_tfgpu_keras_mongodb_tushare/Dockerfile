FROM tensorflow/tensorflow:latest-gpu-py3-jupyter
RUN pip install pandas numpy keras pymongo tushare pyspark
WORKDIR "/app"
CMD ["bash", "-c", "source /etc/bash.bashrc && jupyter notebook --notebook-dir=/app --ip 0.0.0.0 --no-browser --allow-root"]
