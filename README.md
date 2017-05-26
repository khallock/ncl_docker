docker build -t ncl .

docker run -v $PWD:/ncl ncl hello.ncl
