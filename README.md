# Nominatim Docker (for North America)
This is a container for setting up a Nominatim server for geocoding North American addresses. It is
a large dataset and requires over 200GB of hard drive space as of 06/03/2017; also, note that the 
build process may take several days to run to completion.

```
git clone https://github.com/k15z/nominatim-docker
cd nominatim-docker/2.5
docker build -t nominatim .
docker run --restart=always -d -p 8080:8080 nominatim
```
