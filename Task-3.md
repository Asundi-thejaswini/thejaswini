**By Referring to C-based Lab videos and RISC-V-based lab videos**

**Snapshots of the compiled C code and RISC-V**

**Step 1: check whether the leafpad is installed in ur machine by using the commands
leafpad sum1ton.c& (sum1ton.c is the file name)
If the leafpad editor is opened without any errors then type the C code.**
****If the leafpad is not installed in ur machine then install by using the following command**

**sudo snap install leafpad****
![ec5df64a-09d4-45c6-b416-584c9fb5d4f3](https://github.com/Asundi-thejaswini/thejaswini/assets/120015783/94ded5ee-3396-4ccb-b66e-24506141b716)



****Step 2: Writing the C code in the leafpad editor** using the following command

**leafpad sum1ton.c&**
![c83de552-3fc3-40a7-916b-7e7fb7bd24a1](https://github.com/Asundi-thejaswini/thejaswini/assets/120015783/4c93af76-a253-4cf0-b3e6-837786c27521)



**Step 3: After writing the C code save the editor by Ctrl+s**

**Step 4: Check for the errors by using the following command(compilation step)**

**gcc sum1ton.c**
![ec5df64a-09d4-45c6-b416-584c9fb5d4f3](https://github.com/Asundi-thejaswini/thejaswini/assets/120015783/2f7ac760-7db4-4712-9c04-cede6f200a53)


**Step 5: Check the output by using the command**

**./a.out**
![ec5df64a-09d4-45c6-b416-584c9fb5d4f3](https://github.com/Asundi-thejaswini/thejaswini/assets/120015783/95cc3571-bab9-4316-a44c-720a5b9742db)




**The results will be displayed as** 

**Sum of numbers from 1 to 500 is 125250**


********************************************************RISCV Compilation and Execution*****************************************************

**Step 1: View the C Code in the editor window using the following command**

**cat sum1ton.c**
![f9e4fb36-5922-4bef-b2b5-10f10d71ad8a](https://github.com/Asundi-thejaswini/thejaswini/assets/120015783/8a92d80e-1ea4-4ed1-a264-dee2ffc3755b)



**Step 2: Compile the code in riscv using the following command**

**riscv64-unknown-elf-gcc -O1 -mabi=lp64 -march=rv64i -o sum1ton.o sum1ton.c**

![c32a7a15-b5a7-4673-9db3-e48209c24fdc](https://github.com/Asundi-thejaswini/thejaswini/assets/120015783/ab0cdbc7-bc6f-41be-b8ca-6d4e5d5763df)


**Step 3: The ls ltr command in Linux is used to list the contents of the current directory in long format, sorted by last modified time in reverse order.**

**use the command**

**ls -ltr sum1ton.c**
![c32a7a15-b5a7-4673-9db3-e48209c24fdc](https://github.com/Asundi-thejaswini/thejaswini/assets/120015783/0ac9e9eb-b3dc-4b37-a1ef-025ab218eb16)


![bed71df7-3ad4-49fc-9a61-99d5cbd348da](https://github.com/Asundi-thejaswini/thejaswini/assets/120015783/2197bcd4-5a3c-46f8-85ba-8d4b75b84046)


**Search for the Main and check the instructions of the C code execution. It has 15 instructions in the C execution**

![22acf71d-53c4-4cf7-9c14-6f4a53d7b50e](https://github.com/Asundi-thejaswini/thejaswini/assets/120015783/32075673-cb27-4a9f-a8a6-1cae841c10a8)

![ed512214-bca6-440e-b863-0ffabab4b78d](https://github.com/Asundi-thejaswini/thejaswini/assets/120015783/ebe4a543-2775-4770-a8f1-f25874c580d2)




**Step 4:**

**riscv64-unknown-elf-gcc -Ofast -mabi=lp64 -march=rv64i -o sum1ton.o sum1ton.c**
![20492d85-23c5-4810-a039-5a27a98e977e](https://github.com/Asundi-thejaswini/thejaswini/assets/120015783/2655168b-8065-4d90-8118-3a6014037e0b)

![ec3803e4-ab24-446e-abff-0710f024933d (1)](https://github.com/Asundi-thejaswini/thejaswini/assets/120015783/0fdc5237-8229-4f13-b9f8-e1f81db6f378)





