# adding copy building files

COPY ./ ./

# port mapping  

EXPOSE 8080

docker run -p 8080 : 8080 <image name>
docker run -p 5000 : 8080 <image name>

# working directory
