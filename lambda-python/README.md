open the current directory into our lambda-env docker container environment

docker run --rm -tiv $HOME/.aws:/root/.aws -v ${PWD}:/tmp --name aws-cli-1 aws-cli