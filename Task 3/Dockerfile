FROM python:3.10-slim
WORKDIR /Task3
COPY requirements.txt .
RUN pip install -r requirements.txt
RUN pip install notebook
COPY . .
EXPOSE 8888
CMD ["jupyter", "notebook", "--no-browser", "--ip=0.0.0.0", "--allow-root", "--NotebookApp.token=''", "--NotebookApp.password=''"]