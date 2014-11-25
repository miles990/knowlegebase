###執行以下指令

` sudo docker ps -a | awk '{print $1}' | grep -v CONTAINER | xargs sudo docker rm `  
 
` sudo docker images | grep "<none>" | awk '{print $3}' | xargs sudo docker rmi`