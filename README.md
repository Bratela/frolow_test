# HP Prime calculator with Frolow Test.
Frolow test for calculator HP Prime.

I used this test from this article
http://www.leningrad.su/calc/speed.php

## Calculator HP Prime description:

Software version: 2.1.14603(2021 12 02)

Hardware Version: C

CAS Version: 1.5.0

Serial Number:9CJ71500VS

Operating System:V0.050.640

![HP Prime](/hp_prime2.png)

## Program for test:

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
![HP Prime PPL](/hp_prime1.png)

### Speed:
Iteration was made 1000 times for speed calculation.

1000 iteration = 00:58.18 min

10 iteration = 00:00.5818 min


### Math Result :

674514.86877

4669470.09653

![HP Prime Result](/hp_prime3.png)

#### P.S. 

For screenshot i used HP Prime Connectivity Kit

If you see any mistake or questions please write me or leave comment in this GitHub.

Thank you!
