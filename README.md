# AK.Lab5 (By IO-11 Yehor Seniuk)
```bash
insmod hello.ko p=5
```
![alt](normal_workflow.jpg)
```bash
insmod hello.ko p=8
```
![alt](oops_message.jpg)
```bash
arm-linux-gnueabi-objdump -dS hello.o | cat | grep “e7f001f2” -B 5 -A 5
```
![alt](error_place.jpg)
