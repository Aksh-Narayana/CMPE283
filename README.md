# CMPE 283 - Assignment 1

>> By Akshara Narayana and Abhinav Kashyap Mandula

 We used Akshara's GCP to work on this assignment.


### Akshara's Contribution

I watched the lecture video with Abhinav, and we both followed the instructions to find the nested virtual machine's vmx features. I established an instance of the Intel Cascade Lake Architecture n2-standard-2 after signing up with Google Cloud for this. I installed the make module to execute the professor's files and adjusted the setup of the current VM to support nested virtualization. I I nserted the newly built modules in the kernel and displayed the considered register's features.

### Abhinav's Contribution

Akshara and I collaborated on this project. We checked and noted the assignment's specifications & rubric and went over the lecture recording's specifications. I extracted the starter.c file and makefile from her GCP, added the extra structs, and defined the various capability info sections. I increased the calls to report capability as well as the remaining reads of the msrs for each capability in the detect vmx features function. By running make and then sudo insmod on the freshly created.ko file, I attempted to test it.





## Implementation Steps :

##### Step 1: Exported the current configuration of the files into the 'vmx-features.yaml' yaml file


##### Step 2: Updated the configuration file with details about nested virtualization

<img width="466" alt="step 2 final" src="https://user-images.githubusercontent.com/99699489/200482922-8060a892-ce55-4bde-8bfa-c878ec988c27.png">




##### Step 3: Updated the VM configuration


##### Step 4: Determining if VM virtualization is activated: getting anything other than 0 indicates the nested virtualization is activated.

<img width="450" alt="step 4 final" src="https://user-images.githubusercontent.com/99699489/200483095-0d1cae32-f599-4fa8-acc4-1cbc9e688c75.png">




##### Step 5: To print the vmx feature of the register and the make file, cloned the git repository using the professor's program. Also, Installing the make module using the below command.

<img width="461" alt="step 6 finallll" src="https://user-images.githubusercontent.com/99699489/200483257-729fe198-858f-4c54-95b1-8e7b8a001b54.png">




##### Step 6: Installed the linux header of the current kernel to run the make command. Run the make command, use insmod to insert the module to the kernel, and display the features of the considered register.

<img width="468" alt="step 8 3 is mana step 6 1" src="https://user-images.githubusercontent.com/99699489/200483494-fbaaafff-1c8c-42df-8715-08c8007f3948.png">



##### Step 7: After adding the remaining structs and definitions, you'll see the below output

![final 1 1 (2)](https://user-images.githubusercontent.com/99699489/200483978-6ee77f15-f919-43da-a030-d5069cf716fb.png)


![final 1 2](https://user-images.githubusercontent.com/99699489/200484006-6f107f12-c130-4115-af52-c8d35fe99560.png)


![final 1 3](https://user-images.githubusercontent.com/99699489/200484070-e30e5cfb-6f5c-4a40-87a9-7408077ab876.png)




#### Reference for checking secondary processor

<img width="646" alt="image" src="https://user-images.githubusercontent.com/99863530/200481568-5ddf0817-c528-4a3f-97c6-22753e63402f.png">



##### Reference for Checking Tertiary processor

https://patchwork.kernel.org/project/kvm/patch/20220225082223.18288-2-guang.zeng@intel.com/





