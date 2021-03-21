---
layout:     post
title:      Have a donut.
subtitle:   要不，来一个甜甜圈？
date:       2006-09-15
author:     a1k0n
header-img: img/2006/09/15/01/title.jpg
catalog: true
tags:
    - Donut
    - C
---

(compile with `gcc -o donut donut.c -lm`, and it needs ANSI- or VT100-like emulation)

```c
            k;double sin()
         ,cos();main(){float A=
       0,B=0,i,j,z[1760];char b[
     1760];printf("\x1b[2J");for(;;
  ){memset(b,32,1760);memset(z,0,7040)
  ;for(j=0;6.28>j;j+=0.07)for(i=0;6.28
 >i;i+=0.02){float c=sin(i),d=cos(j),e=
 sin(A),f=sin(j),g=cos(A),h=d+2,D=1/(c*
 h*e+f*g+5),l=cos      (i),m=cos(B),n=s\
in(B),t=c*h*g-f*        e;int x=40+30*D*
(l*h*m-t*n),y=            12+15*D*(l*h*n
+t*m),o=x+80*y,          N=8*((f*e-c*d*g
 )*m-c*d*e-f*g-l        *d*n);if(22>y&&
 y>0&&x>0&&80>x&&D>z[o]){z[o]=D;;;b[o]=
 ".,-~:;=!*#$@"[N>0?N:0];}}/*#****!!-*/
  printf("\x1b[H");for(k=0;1761>k;k++)
   putchar(k%80?b[k]:10);A+=0.04;B+=
     0.02;}}/*****####*******!!=;:~
       ~::==!!!**********!!!==::-
         .,~~;;;========;;;:~-.
             ..,--------,*/
```

(This was my first attempt at obfuscated C and I feel it's pretty amateurish; see [Donut Mark II](http://panzhifei.fun/2006/09/20/obfuscated_c_donut_2/) for a more impressive demo — though this one is simple and elegant in comparison.)
