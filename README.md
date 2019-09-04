# Easticsearch image for Bitbucket Pipelines

Bitbucket pipelines does not allow you to use dot notation in variables. So I created my own elastic search docker image to include the discovery type.

## Version
* Elasticsearch 7.1.1

## Repos
* https://bitbucket.org/lionslair/elasticsearch-bitbucket-pipelines
*


## Test and build

`docker build -t elasticsearch-bitbucket-pipelines .`

When you commit to the bitbucket repo it will then trigger the image to be rebuilt on dockerhub.

Run the container locally after building.

`docker run -i -t -P elasticsearch-bitbucket-pipelines:latest /lib/systemd/systemd`
