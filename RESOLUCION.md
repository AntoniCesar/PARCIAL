RESOLUCION
================
ANTONI\_ESQUIVEL
24/7/2021

### PREGUNTA 1.1

``` r
r <- NULL; y <- NULL
a <- c(1000,1500,2000,2500,3000)
for (i in a) {
  y <- ((-0.004*i) + 85.4); r <- c(r, y)
}

r
```

    ## [1] 81.4 79.4 77.4 75.4 73.4

### PREGUNTA 1.2

``` r
T.D <- matrix(c(3,2,1,2,-1,4,-2,3,2), ncol=3,nrow=3)
T.I <- c(0,9,-4)
Solución <- solve(T.D,T.I)
names(Solución) <- c("x","y","z")
Solución
```

    ##  x  y  z 
    ##  2 -2  1
