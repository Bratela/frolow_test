# HP Prime calculator with Frolow Test.
Frolow test for calculator HP Prime
I used this test from this article
http://www.leningrad.su/calc/speed.php

## Calculator HP Prime description:

Software version:2.1.14603(20121 12 02)

Hardware Version: C

CAS Version: 1.5.0

Serial Number:9CJ71500VS

Operating System:V0.050.640

## Programm for test:

### Language: HP PPL

```
#pragma mode( separator(,;;) integer(b32) )
EXPORT FROLOW_TEST()
BEGIN
FOR D FROM 1 TO 1000 DO

LOCAL A:=1,0000001;
LOCAL B:=A;
 
 FOR C FROM 1 TO 27 DO
  A:= A*A;
  B:= B^2,01

 END;
 
PRINT(A);
PRINT(B);
PRINT("------------");
END;
END;

```
