# Welcome to the Anythink Market repo

To start the app use Docker. It will start both frontend and backend, including all the relevant dependencies, and the db.

Please find more info about each part in the relevant Readme file ([frontend](frontend/readme.md) and [backend](backend/README.md)).

## Development

When implementing a new feature or fixing a bug, please create a new pull request against `main` from a feature/bug branch and add `@vanessa-cooper` as reviewer.

## First setup

**[TODO 05/01/2018 @vanessa-cooper]:** _It's been a while since anyone ran a fresh copy of this repo. I think it's worth documenting the steps needed to install and run the repo on a new machine?_

## Setting up Environment

It requires setting up a local environment to keep using this project.

Steps to be followed:

### 1. Cloning the git repo

To copy the required repo run the following command on the local system.
```sh
git clone https://github.com/ObelusFamily/Anythink-Market-vs56w.git
```
### 2. Installation of Docker
Follow this link [Install Docker](https://docs.docker.com/get-docker/) to Download the Docker on respective platform.

If you are a Windows User, You might face some issues. It may ask you to download manual linux kernel.  Follow  [this link](https://docs.microsoft.com/en-us/windows/wsl/install-manual#step-4---download-the-linux-kernel-update-package) to download and install. 

### 3. Running Some Commands to build Environment
After Successfull installation of Docker.Run following command
```sh
 docker -v  
 
 docker-compose -v
```
to verify docker is  ready.  Now it's time to Run 
```
docker-compose up
```
 from the project root directory that you have cloned. It will take some time to configure the system.
 
If Docker is working correctly, the backend should be running and able to connect to your local database.
Let's test this by pointing your browser to
```sh
http://localhost:3000/api/ping
```
Now, it’s time to check the frontend and make sure it’s connected to the backend.
If everything is working properly, you’ll be able to create a new user on
```sh
http://localhost:3001/register
```
