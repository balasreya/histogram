# histogram
names<-c("nell","fell","gell","ull")
gender<-c("male","female","male","male")
print("enter the marks")
marks<-scan()
dataframes=data.frame(names,gender,marks)
write.csv(dataframes,"marks",row.names=FALSE)
x=read.csv("marks")
print(x)
hist(x$marks,
       xlab="assingment marks",
       ylab="frequency of student",
       main="rvr&jc 2020-2024",
       xlim=c(0,7),
       breaks=9,      
       col=rainbow(length(names)))

