# HELLO WORLD JAVA POO

# COMPILE PC
javac -cp src -d build src/Hello.java

# RUN PC
java -cp build Hello

# COMPILE ANDROID [ ECJ ]
ecj -cp src -d build src/Hello.java
cd build
dx --dex --output=hello.jar Hello.class
cd ..

# RUN ANDROID [ DALVIK VM ]
dalvikvm -cp build/hello.jar Hello
