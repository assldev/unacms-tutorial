# How to deploy UNA CMS?
1. Setup Una Application Server
2. Setup mySQL Database Server
3. Install Una Application
4. Configure

## Setup Un Application Server
1. Clone this repository for Dockerfile at the machine you want to install the application server.
2. Download Una source code.
3. Build docker image.
4. Run the docker container.
5. Make sure the server is running properly.

## Setup mySQL Database Server (using docker)
You could use any mySQL database server setup. I'll be using mySQL on [Digital Ocean](https://m.do.co/c/e0a32d405649) (referral link) for this. It s pretty straightforward, tutorial is [here](https://docs.digitalocean.com/products/databases/mysql/how-to/).

## Install Una Application
Just go through the wizard as it says. You will have to create an account on [unacms.com](unacms.com) for a key and secret during the process.

## Configure
Lots of configuration options in Una. Find their details [here](https://unacms.com/wiki/Studio).