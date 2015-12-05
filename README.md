docker build -t minerapp/ip-service --no-cache .
docker run -t -d -e PORT=5000 --expose 5000 --net=host minerapp/ip-service /bin/sh -c ./run.sh
