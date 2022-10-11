
# Micro-Services

A project using micro-services architecture using following technologies.
- Protocol Buffers
- gRPC
- Core python
- Flask 


### Project Requirements
```
 Docker
```

### Project Setup
- Clone the Project
- Go to the `recommendations` driectory and type following 
  ```
   python -m grpc_tools.protoc -I ../protobufs --python_out=. \
        --grpc_python_out=. ../protobufs/recommendations.proto
   ```
- Now go to `marketplace` directoy and type same python command there. This will create two new file in both directories. 
- Now Type `docker-compose up ` or `docker-compose up --build` if you are building project for the first time.
- Now go to the browser and type `127.0.0.1:8000` and your project is up and running.
