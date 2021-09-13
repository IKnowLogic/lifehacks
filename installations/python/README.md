*Guide for installing python (specific version) on linux*

Install Required libraries  
`$ sudo apt-get install libssl-dev openssl make gcc`  

Go to opt directory and wget python version:  
Find the python version here: https://www.python.org/ftp/python/  
`$ cd /opt  
 $ wget https://www.python.org/ftp/python/3.9.2/Python-3.9.2.tgz`  

Extract Archive  
`$ tar xzvf Python-3.9.2.tgz`  

cd into python directory  
`$ cd Python-3.9.2`  

Compile new version  
`$ ./configure  
 $ make  
 $ make install  
`  

Create symlink  
` $ sudo ln -fs /opt/Python-3.9.2/Python /usr/bin/python3.9`  

Check python version  
` $ python3.9 --version`  