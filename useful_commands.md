
# GIT
***
#### Selectively merge files from one branch into another
`git merge --no-ff --no-commit <branch to merge from>`
#### Checkout and track a remote branch locally
`git checkout -b <local branch name> <remote branch name>`
`(e.g. git checkout -b local-branch remotes/origin/remote-branch-name)`
#### Add changes to commit
`git add <changed file 1> <changed file 2>`
`or	 git add --all`
#### Push local changes to its tracking remote branch
`git push origin HEAD:<remote-branch-name>`
#### Create and tag a release
`git tag -a <tag #> -m "Tag for release <tag #>"`
    

# DOCKER
***
#### Prune all docker volumes
`docker volume prune`
#### Prune docker system (containers & volumes)
`docker system prune -a`
#### Kill all running docker containers
`docker kill $(docker ps -q)`
#### Tail docker container's logs 
`docker tail -f <container name>`
#### Open a CLI for a docker container
`docker exec -it <container name> bash`
#### Copy docker container files to local machine
`docker cp <container name>:<file path> <local file path>`
    

# KAFKA
***
#### Tail a kafka topic 
`kafka-console-consumer --bootstrap-server <kafka port> --topic <topic name> --from-beginning`
`kafka-console-consumer --bootstrap-server <kafka port> --topic <topic name>`
#### List kafka topics
`kafka-topics --list --zookeeper zookeeper:<zookeeper port>`
    
    
# REDIS
***
#### Open redis CLI
`docker exec -ti docker_cloud-data-sink-pef-redis_1 redis-cli`
#### List all keys
`keys *`
#### Return data for a specific hash
`hgetall [hash]`
#### Move a Key into a seperate database
`move [key] [db#]`
#### Flush all keys from all databases
`flushall`
#### Flush all keys from the current database
`flushdb [db#]`




