### ENTRYPOINT

Entrypoint is also used to run the container just like CMD but there are few differences

1. We can not override ENTRYPOINT, we can override CMD
2. We can not override ENTRYPOINT if you try to do so it will got and append to ENTRYPOINT command
3. If you use CMD and ENTRYPOINT and dont give any command from terminal CMD acts as argument provider to ENTRYPOINT
4. If you dont provide any argument through the run time then ENTRYPOINT by default take argument from CMD, If you provide argument during the runtime it will override the CMD command.
5. CMD will supply default arguments to ENTRYPOINT
6. You can always override CMD arguments from Runtime
