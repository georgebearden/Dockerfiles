To create a new set of AWS credentials from the docker image and store locally on host machine
`docker run --rm -tiv $HOME/.aws:/root/.aws aws-cli aws configure`

To run the aws-cli image and mount the credential file
`docker run --rm -tiv $HOME/.aws:/root/.aws --name aws-cli-1 aws-cli`

To remove the aws-cli-1 container
`docker rm $(docker ps -a -q --filter="name=aws-cli-1")`