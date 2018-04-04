# cdd
"cdd" is a shortcut "cd" jump to your most frequently used directory. Very useful if you are opening up new terminals and dealing with ```cd /to/a/very/far/away/directory```; especially for developers compiling/running program on console.

# Usage
To save a path first, ```cd``` there; then save it with ```cdd -s```  
```
$ cd Documents/development/cpp/apps/example/
$ cdd -s
Path saved!
```
Now you can jump there from anywhere just typing ```cdd```.
```
$ pwd
/home/linus
$ cdd
$ pwd
/home/linux/Documents/development/cpp/apps/example/
```
This example demonstrates jumping to a previously saved path from home directory.

# Installation
1) First, download the script as a zip or using ```git``` like:  
```$ git clone https://github.com/ASR-Lab/cdd```  
    
2) Then give it executable rights:  
```$ chmod +x cdd```
  
3) Then copy/move it to an executable's path e.g:  
```$ sudo mv cdd /usr/bin```
  
4) Last step; add an ```cdd``` alias to ```.bashrc``` (This is needed because a script cannot ```cd``` otherwise.)  
```$ echo "alias cdd='. cdd'" >> ~/.bashrc```  
  
Now, logout and login again to see the effect through your all environment. Or reboot. Or just ```$ source .bashrc``` for testing in the current present terminal.
