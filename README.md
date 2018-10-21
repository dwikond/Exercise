# Exercise
#Dwiko Nugroho Dani (17523115)
#Rio Galang Jati R (17523118)

#Limit
library(Ryacas)
x <- Sym("x") # define x as a symbolic variable
Limit(1-(cos(x))/x, x, 0)

h <- Sym("h") # define h as a symbolic variable
Limit(2*(-3+h)^2-18/h, h, 0)

t <- Sym("t") # define t as a symbolic variable
Limit(t-sqrt(3*t+4)/4-t, t, 4)

#Differentiation
#1.
library Ryacas
x <- Sym("x")
Simplify(deriv(sqrt(x)*(x+1),x))

#2.
library(Ryacas)
x <- Sym("x")
Simplify(deriv(2*x^2-3/sqrt(x), x))

#3.
library(Ryacas)
x <- Sym("x")
Simplify(deriv(x-1/x+1), x)

#4.
integrand <- function(x){
return((2*x+(x+1))/(2*root(x,2)))
}

integrand <- function(x){
return((8*x^2+(-2*x^2+3))/(2*root(x,2)))

integrand <- function(x){
return(2/(x^2+2*x+1))
}

#Integration
#No1
f1 <- function(x){
   result <- 2*x^3
}
integrate(f1,0,3)

#No2
f2 <- function(x){
   result <- 1-(5*x^4)
}
integrate(f1,-1,2)

#No3
f3 <- function(x){
   result <- x^4-(3*x^2)+5
}
integrate(f3,-2,2)

#No4
f4 <- function(x){
   result <- x^2+1/(2*sqrt(x))
}
integrate(f4,1,4)

#No5
f5 <- function(x){
   result <- x*(2-3*x)^2
}
integrate(f5,0,2)
