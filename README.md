# zowe-docker
Build Docker images for zowe-cli

docker file and entry point provided by https://medium.com/zowe/running-zowe-cli-on-jenkins-with-docker-7fd35d4211d0

Run command:
docker run --name=zowe-cli --cap-add ipc_lock --rm -it -d --mount type=bind,source="$PWD",target=/workspace,consistency=delegated zowe-cli