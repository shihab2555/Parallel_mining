# Parallel_mining
Please follow the instruction  below to setup the environment. This is prepared for Ubuntu operating system.

Check the system is up to date.
sudo apt-get update
sudo apt-get -y upgrade

Get GoLang
wget https://dl.google.com/go/go1.11.4.linux-amd64.tar.gz
sudo tar -xvf go1.11.4.linux-amd64.tar.gz
sudo mv go /usr/local

Export the path
export GOROOT=/usr/local/go
export GOPATH=$HOME/Projects
export PATH=$GOPATH/bin:$GOROOT/bin:$PATH

Install the library
go get github.com/davecgh/go-spew/spew
go get github.com/gorilla/mux
go get github.com/joho/godotenv
go get -d github.com/libp2p/go-libp2p/...

Go to the root folder
make
make deps

We recommend to write/modify the code in the path go\src\github.com\libp2p\go-libp2p\examples\P2P. If there is no P2P folder under example, create it.

Please run the following command again before you run the code in root folder.
make
make deps
----------
