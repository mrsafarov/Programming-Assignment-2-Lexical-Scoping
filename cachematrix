makeCachematrix<-function(x=matrix()){
    inver<-NULL
    set<-function(y){
        x<<-y
        inver<-NULL
    }
get<-function()x
setinver<-function(inverse) inver<-inverse
getinver<-function()inver
list(set=set, get=get,setinver=setinver, getinver=getinver)
}

cacheSolve<-function(x,...) {
    inver<-x$getinver
    if(!is.null(inver)){
       message('Getting data')
    return(inver)}

dat<-x$get
inver<-solve(dat,...)
x$settinver(inver)
inver
}
