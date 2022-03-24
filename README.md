# nncase


## Build from source
```
$ docker buildx build . --tag=nncase:latest --platform linux/amd64 -f Dockerfile.source
$ docker run --it --rm --platform linux/amd64 nncase:latest
```

## Build from package
```
$ docker buildx build . --tag=nncase:1.4.0 --platform linux/amd64 -f Dockerfile.1.4.0
$ docker run -it --rm --platform linux/amd64 -v ${PWD}/nncase/examples:/mnt nncase:1.4.0 python3 Compile_float32_model_for_tflite.py /mnt/20classes_yolo/model/20classes_yolo.tflite
```
