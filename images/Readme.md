## Execution results

## AWS
### Deploying AWS infrastructure
![img-0](0_deploying_aws_infrastructure.png) 

### Checking state of resources in Cloudformation
![img-11](11_checking_state_of_resources_in_cloudformation.png) 

### Checking EKS cluster and Nodes
![img-12](12_checking_eks_cluster.png)

![img-12-1](12_1_checking_eks_nodes.png)

---
## Jenkins Pipeline
### Running pipeline lint step
![img-1](1_running_pipeline_lint_step.png) 

### Running pipeline build and publish Docker image step
![img-2](2_build_and_publish_docker_image_step.png) 

### Docker images in DockerHub
![img-3](3_docker_images_in_dockerhub.png)  

---
## EKS 
### Connecting local machine to EKS
![img-4](4_connect_your_machine_to_eks.png) 

### Getting Nodes of EKS Cluster
![img-5](5_getting_nodes_eks.png) 

### Setting controller blue green
![img-6](6_setting_controllers_blue_green.png) 

### Setting service of load balancer type
![img-6](7_setting_service_load_balancer.png)  

### Getting service deployed
![img](getting_service_deployed.png)

### Checking blue deployment
![img_8](8_checking_blue_deployment.png)

### Doing a change to blue-green-service.json for do green deploy
![img_9](9_doing_a_change_to_blue-green-service-json_file.png) 

### After do: kubectl apply -f blue-green-service.json
![img_10](10_after_do_apply_to_service.png)

### Describing PODs for see how works the updates

Server A
![img_13](13_server_a.png)

Server B
![img_14](14_server_b.png)
