# First Steps in Scala

This repository contains a few smaller projects and notes to learn Scala
as the first programming language. This repository will grow over time
as it serves the purpose of providing little tasks with step by step
instructions to my little sister Sofia.

At first we start with the most important thing: Installing Scala and
executing a _hello world_ program.

_In detail descriptions are tailored to macOS. We are installing Scala system wide for now._

1. Installing [JDK](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html) (Java SE Development Kit) 8
2. Download the [binaries for mac](https://downloads.lightbend.com/scala/2.12.6/scala-2.12.6.tgz) and
3. Unarchive the tar-file in the Downloads folder and copy it the folder to `/usr/local/share/scala/` by executing
```
cp -R ~/Downloads/scala-2.12.6 /usr/local/share/scala/
```
The folder structure should then look like this:
```
.
...
├── share
│   ├── scala
│   │   ├── bin
│   │   ├── doc
│   │   ├── lib
│   │   └── man
...
```

4. Adding Scala to the path:
```
cd ~
nano .bash-profile
```
Enter the following two lines at the end of the file:
```
export SCALA_HOME="/usr/local/share/scala"
export PATH="$PATH:$SCALA_HOME/bin"
```
Use `control+X` to exit the editor (type `Y` after tyting `control+X`). then restart the terminal and run
```
scala -version
```
This should result in an output like:
```
Scala code runner version 2.12.6 -- Copyright 2002-2018, LAMP/EPFL and Lightbend, Inc.
```
4. For running _Hello World_ follow the instructions on [Your first lines of Code](https://www.scala-lang.org/documentation/your-first-lines-of-scala.html) except for chapter _Script it!_

## Getting Started with the Terminal

- open the Terminal on Mac `/Applications/Utilities/Terminal.app`.
- use `cd` to change the directory e.g. `cd ~/Desktop` to go to to the Desktop `cd ..` to go to the home directory from the Desktop.
- use `mkdir` to create a folder e.g. `mkdir hello-world`.
- use `pwd` to see the path of the current directory
