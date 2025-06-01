Homework for StanfordOnline Compiler course


## Installing Directly on Linux

NOTE: We highly recommend using the VirtualBox VM.

However, there was enough demand that we are providing these instructions for people who want to run directly on their own installation of Linux. These instructions were tested with Ubuntu 11.10, but should work on similar (Debian-based) systems, and can be adapted for other distros.

Steps:

1. Install packages (If you only intend to use the C++ version, you don't need the jdk). For Ubuntu:
``` 
sudo apt-get install flex bison build-essential csh openjdk-6-jdk libxaw7-dev`
```

2. Make the /usr/class directory:
```
sudo mkdir /usr/clas
```

3. Make the directory owned by you:
```
sudo chown $USER /usr/class
``` 

4. Go to /usr/class and download the tarball:
```
cd /usr/class
wget https://courses.edx.org/asset-v1:StanfordOnline+SOE.YCSCS1+1T2020+type@asset+block@student-dist.tar.gz
``` 

5. Untar:
```
tar -xf student-dist.tar.gz
``` 

6. If you want things exactly like the VM:

    1. Add a symlink to your home directory:
    ```
    ln -s /usr/class/cs143/cool ~/cool
    ``` 

    2. Add the bin directory to your $PATH environment variable. If you are using bash, add to your .profile (or .bash_profile, etc. depending on your configuration; note that in Ubuntu have to log out and back in for this to take effect):

    ``` 
    PATH=/usr/class/cs143/cool/bin:$PATH
    ``` 