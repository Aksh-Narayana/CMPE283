# CMPE 283 - Assignment 1

>> By Akshara Narayana and Abhinav Kashyap Mandula

 We used Akshara's GCP to work on this assignment.


### Akshara's Contribution

I watched the lecture video with Abhinav, and we both followed the instructions to find the nested virtual machine's vmx features. I established an instance of the Intel Cascade Lake Architecture n2-standard-2 after signing up with Google Cloud for this. I installed the make module to execute the professor's files and adjusted the setup of the current VM to support nested virtualization. I I nserted the newly built modules in the kernel and displayed the considered register's features.

### Abhinav's Contribution





## Implementation Steps :

##### Step 1: Exported the current configuration of the files into the 'vmx-features.yaml' yaml file


##### Step 2: Updated the configuration file with details about nested virtualization

<img width="466" alt="step 2 final" src="https://user-images.githubusercontent.com/99699489/200482922-8060a892-ce55-4bde-8bfa-c878ec988c27.png">




##### Step 3: Updated the VM configuration


##### Step 4: Determining if VM virtualization is activated: getting anything other than 0 indicates the nested virtualization is activated.



##### Step 5: To print the vmx feature of the register and the make file, cloned the git repository using the professor's program. Also, Installing the make module using the below command.



##### Step 6: Installed the linux header of the current kernel to run the make command. Run the make command, use insmod to insert the module to the kernel, and display the features of the considered register.



##### Step 7: After adding the remaining structs and definitions, you'll see the below output




#### Reference for checking secondary processor

<img width="646" alt="image" src="https://user-images.githubusercontent.com/99863530/200481568-5ddf0817-c528-4a3f-97c6-22753e63402f.png">



##### Reference for Checking Tertiary processor

https://patchwork.kernel.org/project/kvm/patch/20220225082223.18288-2-guang.zeng@intel.com/





