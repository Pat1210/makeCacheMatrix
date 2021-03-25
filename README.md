# makeCacheMatrix
My makeCacheMatrix on GitHub
makeCacheMatrix <- function(x = matrix()){
      inv <- NULL
      set <- function(x){
        x <<- NULL
        
        }         
get <- function(){x}
setInverse <-function(inverse){inv <<- inverse}
getInverse <-function(){inv}
list(set = set, get = get, setInvrese= setInvrese, getInverse = getInverse)
}

cachesolve <- function(x,...){
  inv <-x$getInverse()
  if (!is.null(inv)){
    message("getting cached data")
    return(inv)
    }
    matrix() <-x $get()
    inv<-solve(matrix,...)
    x$setinverse(inv)
    inv

  }
