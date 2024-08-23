# grorbits
This is a public source code repository of GROrbits. This is not my code, but permission was granted by the author.

The actual website of the project is http://stuleja.org/grorbits . This
repository is simply making teh code easily available, and reorganizing it
to fit idiomatic Java build systems.

# Instructions.

* Install java https://adoptium.net/es/download/
* Install gradle https://gradle.org/install/

https://stackoverflow.com/questions/52431764/difference-between-openjdk-and-adoptium-adoptopenjdk
https://stackoverflow.com/questions/53272230/could-not-create-service-of-type-scriptpluginfactory-using-buildscopeservices-cr

https://services.gradle.org/distributions/

* run gradlew.bat
* To compile: gradlew jar
  File is generated in build\libs
* To run showing System.out: java -jar grorbits-1.0.jar

# Setttings non rotating black hole

- Program Mode -> Motion -> rain map = 0
- Advanced -> Orbital Trajectory settings -> set increment dt = 0.0001
- Advanced -> Orbital Trajectory settings -> number of data points 4000

# Hacking inspection

- The hacking works by generating a bunch of light orbits based on settings via the GUI:

* dt: used 0.001
* num points: used 10000
* r: used 1.0, 2.0 and 3.0
* settings can be initialized with the two gsc files

* Hacking is done in GROrbits.java triggering the generation of a blip_radius.txt file when clickint "Plot"


# Notes: 
  black hole radius = 2M all related to c=1 and M
  circular orbit at r=3M and b=5.1961524227066045 (in oir out) max b, can not be lower (see potential and forbidden region)

