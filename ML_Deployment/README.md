
Iris Classifier API (with Deployment)
======================================

Make a simple Iris classifier ML model and use FastAPI to make an API for it. Deployed using Docker. Dockerfile and relevant commands included.

------

## Requirements
* Python3.6+
* Rest mentioned in requirements.txt (pip install requirements.txt)

## To run 

1. Model Training
  ```
  $ cd models
  $ python model.py
  ```
2. Start the server
  ```
  $ cd ..
  $ python server.py
  ```
3. Check if server is running from command line 
  ```
  $ python request.py
  ```
4. FastAPI dashboard 
  ```
  Head to http://localhost:8000/docs
  ```
5. Docker image
  ```
  docker build -t iris-ml .
  ```
6. Start Docker container
  ```
  docker run -d -p 8000:8000 --name iris-api iris-ml
  ```

