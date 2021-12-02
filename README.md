## Inverted index using Apache Spark (Pyspark) 

Pull the docker image from docker hub

```sh
docker pull mcr.microsoft.com/mmlspark/release
```
Run the docker image in interactive mode and mount the volume where Data is present so that the data is accessible inside the docker container.

Map the port 8888 to 8888 so that when we run the jupyter notebook in the container, we can access it from the host machine

```sh
docker run -it -v /home/kali/sparkHW5/Data:temp/Data -p 8888:8888 mcr.microsoft.com/mmlspark/release
```
After running the container to launch jupyter notebook, run 
```sh
jupyter notebook
```
Open a web browser and visit localhost:8888 to find the jupyter notebook where we can write and run our pyspark code 
