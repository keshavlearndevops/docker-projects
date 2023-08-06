#Getting Base Image
FROM openjdk:11

# Working Directory where all code will be kept
WORKDIR app/

# copy all conents in current directory from host machine to container
COPY HelloWorld.java .

#compile code
RUN javac HelloWorld.java

#Run Java compiled Code
CMD ["java","HelloWorld"]

