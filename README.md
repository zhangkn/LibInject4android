# LibInject4android
## 整体流程分3步

- 1.在目标进程中分配内存，用来写shellcode和参数
- 2.往目标进程中写入shellcode, shellcode会调用dlopen来载入我们的library
- 3.运行目标进程中的shellcode

- 当然注入是需要root权限:模拟器上可以直接用，但是真机的话，先exploit
