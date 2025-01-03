# Docker-Contenders

# Opencv CUDA Docker cammands
```
1. docker build -t opencv-cuda-latest .
2. docker login
3. docker tag opencv-cuda-latest:latest namdeopatil/opencv-cuda:latest
4. docker push namdeopatil/opencv-cuda:latest
```

## Running the Docker Image Locally
```
1. docker pull namdeopatil/opencv-cuda:latest
2. docker run -it --rm namdeopatil/opencv-cuda:latest
```

## Run with Mounting Volumes
``` docker run -it --rm -v /path/to/local/dir:/path/in/container namdeopatil/opencv-cuda:latest```


## Run with GPU Support (If CUDA is Required) If the image uses CUDA, ensure you have NVIDIA Docker installed and run it with GPU support
```docker run --gpus all -it --rm namdeopatil/opencv-cuda:latest```
