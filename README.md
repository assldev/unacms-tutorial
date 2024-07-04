# How to deploy UNA CMS using `docker`?
1. Setup Una Application Server
2. Setup mySQL Database Server
3. Install Una Application
4. Configure

## Setup Un Application Server
1. Clone this repository for Dockerfile at the machine you want to install the application server.
```sh
    git clone https://github.com/assldev/unacms-tutorial.git
```

2. Build docker image.
```sh
    cd unacms-tutorial
    docker build -f Dockerfile-spacenook -t una-spacenook .
```

NOTES:
- Pick the [release](https://github.com/unacms/una/releases) you wish to download and update the Dockerfile accordingly (URL and folder name). Be extra cautious with the [compatibility](https://unacms.com/wiki/Requirements#php-version) between Una and php versions.
> For this tutorial, I'll be using [UNA v.13.1.0](https://github.com/unacms/una/releases/tag/13.1.0).

3. Run the docker container.
> Please change the exposed port number to your preferred port (e.g. 8080).
```sh
    docker run -d -p 80:80 una-spacenook
```

4. Make sure the server is running properly by visiting the website.

## Setup mySQL Database Server (using docker)
You could use any mySQL database server setup. I'll be using mySQL on [Digital Ocean](https://m.do.co/c/e0a32d405649) (referral link) for this. It s pretty straightforward, tutorial is [here](https://docs.digitalocean.com/products/databases/mysql/how-to/).

## Install Una Application
Just go through the wizard as it says. You will have to create an account on [unacms.com](unacms.com) for a key and secret during the process.

## Configure
Lots of configuration options in Una. Find their details [here](https://unacms.com/wiki/Studio).