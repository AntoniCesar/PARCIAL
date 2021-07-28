RESOLUCION
================
ANTONI\_ESQUIVEL
24/7/2021

``` r
library(tidyverse)
```

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

### PREGUNTA 2.1

``` r
library(readr)
clima <- read_csv("clima.csv")
```

    ## 
    ## -- Column specification --------------------------------------------------------
    ## cols(
    ##   code = col_double(),
    ##   uh_name = col_character(),
    ##   bh_esc = col_character(),
    ##   bh_month = col_double(),
    ##   bh_pc = col_character(),
    ##   bh_er = col_character(),
    ##   bh_rh = col_character(),
    ##   bh_qd = col_character()
    ## )

``` r
View(clima)
```

### PREGUNTA 3.1

``` r
data1 <- read.csv("temperatureDataset.csv")
names(data1)
```

    ##  [1] "DATE"       "qc00000441" "qc00000435" "qc00000765" "qc00000755"
    ##  [6] "qc00000749" "qc00000837" "qc00000830" "qc00000746" "qc00000804"
    ## [11] "qc00000805"
