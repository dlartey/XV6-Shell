# XV6-Shell
A Simple Shell in XV6

This is my implementation of a shell in XV6 which works on XV6: See the project [here](https://github.com/mit-pdos/xv6-riscv)

To run this program please clone the XV6 github above and run these commands on Ubuntu/Linux
```
sudo apt-get update -y
sudo apt-get install git build-essential gdb-multiarch qemu-system-misc gcc-riscv64-linux-gnu binutils-riscv64-linux-gnu -y

git clone https://github.com/mit-pdos/xv6-riscv
cd xv6-riscv

make qemu
```
![image](https://user-images.githubusercontent.com/58071586/160236975-5c463f9f-19a0-4ea9-98eb-85e9688fea0d.png)


Then make sure that the mysh.c is in the user directory of xv6-riscv,i.e in:
```
xv6-riscv/user directory
```

Then locate the makefile in 
```
xv6-riscv directory
```
and add $U/_mysh\ to UPROGS
![image](https://user-images.githubusercontent.com/58071586/160236820-178fefb2-af44-465d-a0ee-23dfe16d4944.png)

Now you can run
```
make qemu
mysh  
```
To test the program
