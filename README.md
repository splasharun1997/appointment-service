# Terraform Repo

## Setup

A sample goapp application is containeraized and deployed on eks with helm charts

##### Commands used:

1. **File structure**:
   * Dockerfile is present in the root directory
   * helm charts have been created and pushed to deployment-config folder
   * Sample templates generated through helm template commands are stored in ./sample_templates.yaml for reference

##### Pipelines:

###### CI:
1. A CI pipeline is created with steps to checkout code, docker build and push to ecr.
2. AWS credentials are stored in repository secrets.
3. Manual trigger is provided for the pipeline.
![alt text](image.png)

##### Screenshots:
1. A CD pipeline is created with steps to checkout code, acquire kube config and run helm upgrade install.
2. AWS credentials are stored in repository secrets.
3. Manual trigger is provided for the pipeline.
![alt text](image-1.png)

![alt text](image-2.png)

![alt text](image-3.png)

![alt text](image-4.png)