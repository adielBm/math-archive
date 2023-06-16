

- compliations 
	- Constructor call must be the first statement in a constructor



downcasting runtime err 
```java
Child a = (Child) (new Parent()); // Parent constactor & run time error
Parent a = (Child) (new Parent()); // Parent constactor & run time error
```

downcasting compliation err 

```java
Child a = new Parent(); // compliation err
```


```java
Parent a = new Child(); 
Child b = a; // compliation err
```



___


