java-wol
========

A simple Java implementation of WOL(Wake-On-Lan).

##Usage
```java
  WOLNode node = new WOLNode("002245bf6c99");
		try {
			node.wakeUP();
		} catch (UnableToWakeUpWOLNodeException e) {
			//TODO: write some code
		}
```

##MAC Address allowed formats
* 11:22:33:AA:BB:CC
* 11-22-33-AA-BB-CC
* 1122.33AA.BBCC
* 112233AABBCC

> **Note:** The letters can be both upper and lower case.


------

## 使用说明

直接java -jar 运行  
> 参数说明：Mac地址 [广播地址] [端口]

如：

```
# java -jar wol4j-1.0.0.jar 22-00-DD-11-44-7A 192.168.1.255
```

> 默认端口是：9


