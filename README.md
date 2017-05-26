docker build -t ncl -f Dockerfile\_debian\_jessie .

docker run -v $PWD:/ncl ncl hello.ncl
