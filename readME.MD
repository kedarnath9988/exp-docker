# Install Docke in ec2 
 using install-docker file by using 
    # curl <raw > | sudo bash 
# docker home directory -> var/lib/docker -> docker files and all 
  this id decided by CIS_banch marking Center for Internet services 
# increasing the storage volume by ing the following commands 

# PORT EXPOSING  OUT SIDE 
docker run -d -p 80:80 --name frontend --network expense frontend:1.0 
# to not expose to outside world 
docker run -d --name backend --network backend:1.0 
# docker networking 
docker network create expense 
docker network ls 
docker network remove expense 
# Docker volumes 
two types: 
# named volumes
if we specify in the yaml file it will creat autometically and the container will autometically utilize the volume 
# unnamed Volumes 
manually we have to creat the directory and nount to the continer explicitilly 
