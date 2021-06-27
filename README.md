# vagrant-two-tier-stack

Sample Vagrantfile for a multi-machine setup - web01, web02 and db01 (mysql)

To use this do the following

```
vagrant up
vagrant ssh web01 (or web02 or db01)
```

Updated the machines to have 2 cores and 2 GB of RAM

NGINX is also installed, so if you'd like to get access to the webserver, do 

```
vagrant share web01 (or web02)
```

Use the URL (*.ngrok.io) to access this. 

Note that for the above command to work you'd need to have the vagrant-share plugin already installed. Also, ngrok is a dependency for the vagrant share to work, so if that is missing. Please install it. For example, on MacOS you can do
```
brew install ngrok
```
