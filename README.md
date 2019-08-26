# Digital Input/Output for Linux User Guide

## Usage


### Read a single pin from DIN via Digital input/output connector



```
$ sudo ./dio-tool --read <Pin Number>
```



The command return message will be



```
$ DIN-<Pin Number> = <1 OR 0>
```

‌

### Write a single pin to DOUT via Digital input/output connector



```
$ sudo ./dio-tool --write <Pin Number> <0 OR 1>
```


The command return message will be



```
$ Set DOUT-<Pin Number> = <1 OR 0>
```

‌

### Read DIN port via Digital input/output connector



```
$ sudo ./dio-tool --read-all 
```



The command return message will be



```
$ DIN Port = <port value>
```

‌

### Set DOUT port via Digital input/output connector



```
$ sudo ./dio-tool --write-all <port value>
```



The command return message will be



```
Set DOUT port = <port value>
```
‌

> Note. The <Pin Number> range is between 1 to 8. It corresponds Digital Input/Output connector.  If the param isn't correct, dio-tool command will not be executed.
>
> The dio-tool command needs root permission because SMBus BAR's permission supplied by linux kernel is accessed only by root.