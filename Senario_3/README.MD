I have shared sample sample springboot microservice Dockerfile.
THe docker image can be built by using docker build either via Jenkins or any CLI console
Command to build docker image: " docker build -t service . "

OR

docker build -t Mservices .
docker tag Mservices:latest <XXX.dkr.ecr.us-east-2.amazonaws.com/springboot-Mservices:Mservices_$TAG or ${build_id}
docker push XXX.dkr.ecr.us-east-2.amazonaws.com/springboot-Mservices:Mservices_$TAG or ${build_id}

- And the image can be deployed to EKS or ECS by necessary cloud specific steps.

- Attached ECS_Deployment_Script for releasing docker images into AWS ECS
