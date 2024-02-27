**By Referring to C-based Lab videos and RISC-V-based lab videos**

**Snapshots of the compiled C code and RISC-V**

**Step 1: check whether the leafpad is installed in ur machine by using the commands
leafpad sum1ton.c& (sum1ton.c is the file name)
If the leafpad editor is opened without any errors then type the C code.**
****If the leafpad is not installed in ur machine then install by using the following command**

**sudo snap install leafpad****
![abfeaac4-90db-4b98-b24d-0ad2335fbdf6](https://github.com/Asundi-thejaswini/thejaswini/assets/120015783/0983d61c-b74f-402e-ac89-0dc6553005e8)



****Step 2: Writing the C code in the leafpad editor** using the following command

**leafpad sum1ton.c&**
![c83de552-3fc3-40a7-916b-7e7fb7bd24a1](https://github.com/Asundi-thejaswini/thejaswini/assets/120015783/4c93af76-a253-4cf0-b3e6-837786c27521)



**Step 3: After writing the C code save the editor by Ctrl+s**

**Step 4: Check for the errors by using the following command(compilation step)**

**gcc sum1ton.c**
![c83de552-3fc3-40a7-916b-7e7fb7bd24a1](https://github.com/Asundi-thejaswini/thejaswini/assets/120015783/4a207193-fd4d-4d9a-a02e-2023f6b1eb5a)


**Step 5: Check the output by using the command**

**./a.out**
![c83de552-3fc3-40a7-916b-7e7fb7bd24a1](https://github.com/Asundi-thejaswini/thejaswini/assets/120015783/1819ea4c-38a5-4299-a5fc-3153f38e3a3c)



**The results will be displayed as** 

**Sum of numbers from 1 to 500 is 125250**


********************************************************RISCV Compilation and Execution*****************************************************

**Step 1: View the C Code in the editor window using the following command**

**cat sum1ton.c**
![c83de552-3fc3-40a7-916b-7e7fb7bd24a1](https://github.com/Asundi-thejaswini/thejaswini/assets/120015783/33f55be9-e4a8-4c86-ab45-ec3a76e0a5e3)



**Step 2: Compile the code in riscv using the following command**

**riscv64-unknown-elf-gcc -O1 -mabi=lp64 -march=rv64i -o sum1ton.o sum1ton.c**
![c32a7a15-b5a7-4673-9db3-e48209c24fdc (1)](https://github.com/Asundi-thejaswini/thejaswini/assets/120015783/4b373881-834d-404d-8e04-2829cfacff32)



**Step 3: The ls ltr command in Linux is used to list the contents of the current directory in long format, sorted by last modified time in reverse order.**

**use the command**

**ls -ltr sum1ton.c**
![c32a7a15-b5a7-4673-9db3-e48209c24fdc (1)](https://github.com/Asundi-thejaswini/thejaswini/assets/120015783/8b196e37-d5c3-4782-9461-33707908120a)

![c32a7a15-b5a7-4673-9db3-e48209c24fdc (1)](https://github.com/Asundi-thejaswini/thejaswini/assets/120015783/fd33f463-6c87-4a6e-b3a0-d1ab809ce9fa)



**Search for the Main and check the instructions of the C code execution. It has 15 instructions in the C execution**

![22acf71d-53c4-4cf7-9c14-6f4a53d7b50e](https://github.com/Asundi-thejaswini/thejaswini/assets/120015783/b5732dfe-e939-4cea-aea3-91a406ad90da)


![ed512214-bca6-440e-b863-0ffabab4b78d](https://github.com/Asundi-thejaswini/thejaswini/assets/120015783/aa7c080e-d2ca-4775-b344-1dc2a7c643b8)



**Step 4:**

**riscv64-unknown-elf-gcc -Ofast -mabi=lp64 -march=rv64i -o sum1ton.o sum1ton.c**
![866a985b-fb26-429e-9ca5-39f081194087](https://github.com/Asundi-thejaswini/thejaswini/assets/120015783/e247e929-4cbf-4a73-b18d-6c7417c84723)


![9cf91f74-35e7-4777-b7b4-06a444850bb3](https://github.com/Asundi-thejaswini/thejaswini/assets/120015783/1cdcace5-874c-4117-bc7c-94d512fbd734)






