### STOPSIGNAL

STOPSSIGNAL is used to how to exit the container
* By default docker request for exit and wait for some time * If it is not exiting then it can force kill
* when your container received STOPSIGNAL your application can perform
1. you can close DB connection
2. You can do some backup
