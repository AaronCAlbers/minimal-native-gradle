# minimal-native-gradle
Minimal Native Gradle Build Project Setup and Configuration for all Platforms

This project contains a simple C++ Hello World application and The Gradle Wrapper for 4.0.1. The project uses all the default configuration and is the absolute minimal setup I could think of for all platforms.

## Windows

This configuration was tested on a fresh install of Windows 10 with the latest updates.

1. Install Java Runtime Enviroment (JRE) 7 or higher. I recommend using Ninite to get [Java 8](https://ninite.com/java8/ninite.exe).
2. Install [Visual C++ 2015 Build Tools](http://landinghub.visualstudio.com/visual-cpp-build-tools).
3. Download this minimal project or any other mproject that uses The Gradle Wrapper.
4. Run "gradlew build" from the command line where the wrapper lives.

## Mac OS X

This configuration was tested on a fresh install of Mac OS X Sierra 10.12 with the latest updates.

1. Install [Homebrew](https://brew.sh/). Homebrew will automatically install the necessary toolchain and allow for easy install of the JRE.
2. Run "brew cask install java" from the terminal to get Java. (Gradle can be installed directly via Hombrew but this is a minimal setup)
3. Download this minimal project or any other project that uses The Gradle Wrapper.
4. Run "./gradlew build" from the terminal where the wrapper lives.

## Linux

This configuration was tested on a fresh install of Kubuntu 17.04 x64 with the latest updates.

1. Run "java -version" to see if a supported version of Java is already installed (1.8.0_121 or higher). If not:
    1. Run "sudo apt-get install software-properties-common python-software-properties" to get "add-apt-repository" command.
    2. Run "sudo add-apt-repository ppa:webupd8team/java" to add the Java repository.
    3. Run "sudo apt-get update" to update the installer cache.
    4. Run "sudo apt-get install oracle-java8-installer" to install Java.
2. Run "sudo apt-get install g++" to install the toolchain.
3. Download this minimal project or any other project that uses The Gradle Wrapper.
4. Run "./gradlew build" from the terminal where the wrapper lives.
