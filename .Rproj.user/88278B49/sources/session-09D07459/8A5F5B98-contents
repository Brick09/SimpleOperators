install.packages("devtools")
install.packages("roxygen2")
install.packages("rlang")
library(devtools)
library(roxygen2)
library(rlang)

sqrt.2 = function(x){
  if (x<0){
    rlang::abort(message="Error: negative input, NA introduced!")} else{return(sqrt(x))}}

log.2 = function(x){
  if (x<0){
    rlang::abort(message="Error: negative input, NA introduced!")} else{return(log(x))}}

f_operator = function(f){
  force(f)
  function(x){
    if(x>0){f(x)}
    else{catch_cnd(abort(message = "negative input detected", .sublass="invalid_input", invalid_input=x))}}}
