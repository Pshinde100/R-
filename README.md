# R-
My R programming
#Factors#

x <- factor(c("yes","yes","no","yes","no"))
x
table(x)

x1 <- factor(c("yes","yes","no","yes","no"), levels = c("yes","no"))
x1

#Missing Values#

x_na <- c(1,2,NA,10,3)
is.na(x_na)
is.nan(x_na)
x_nan <- c(1,2,NaN,NA,4)
is.na(x_nan)
is.nan(x_nan)

#Data Frames#

x_df <- data.frame(foo = 1:4, bar = c(T,T,F,T))
x_df
nrow(x_df)
ncol(x_df)

#Names#

##Vector##


x <- 1:3
names(x)
names(x) <- c("foo","bar","norf")
x
names(x)

##List##


x_L <- list(a = 1, b = 2, c = 3)
x_L
x_L$a
x_L$b
x_L$c
x_L[2]
x_L[[2]]


##Matrix##

m <- matrix(1:4, nrow = 2, ncol = 2)
m
dimnames(m) <- list(c("a","b"),c("c","d"))
m
