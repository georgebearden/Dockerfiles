Create a new network 
`docker network create redis-network`

Start the server
`docker pull redis`
`docker run --name redis1 -it --net=17006bf9b4d2 -p 6379:6379 redis`

Stop the server
`docker rm $(docker ps -a -q --filter="name=redis1")`

Start the cli (from this directory in the git repo)
`docker run -it --name redis-cli1 --net=17006bf9b4d2 redis-cli /bin/bash`
`redis-cli -h redis1 -p 6379`

Stop the cli
`docker rm $(docker ps -a -q --filter="name=redis-cli1")`

Monitor all commands being sent to the server
`redis-cli -h redis1 -p 6379 monitor`