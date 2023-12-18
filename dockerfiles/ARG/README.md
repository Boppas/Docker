### ARG

Arg is used to supply few variables during the image creation

The first instruction ot use in a dockerfile is always FROM but there is an exception we can use ARG

## ARG is the only instruction we can be us before FROM. ARG declared before can't be accessed after FROM

docker build -t arg:v1 --built-arg VERSION=[the version we want to use]

## USING ENV AND ARG FOR BEST RESULTS
* Create one ENV variable ans assign the value of ARG to that then you can access ARG values through ENV both in image and container
