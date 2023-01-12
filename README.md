# NetCache_2023
Electrical and Computers engineering - 4th year project

Update Background

Setting the enviroment:
option 1 - Recommended
1. Open https://github.com/opennetworkinglab/ngsdn-tutorial and clone the repository using "git clone -b advanced https://github.com/opennetworkinglab/ngsdn-tutorial".
2. Follow the installation guide in the Readme, use "Option 2 - Manually install Docker and other dependencies".
3. This tutorial contains several exercice, some of the are irrelavant to our project.
   Yet, in order to make sure that the setup of the enviroment will work we suggest coping all the files in the "solutions" repository to the                corresponding place in the main repository "ngsdn-tutorial".
   However, we highly recommend following the steps in Exercise 7 ןn order to gain a deeper understanding of the process.
 4. 


option 2
This is an explanation in case the link above doesnt work. 
We advice using the first option because the git provides more details that helps understanding the process.
However, if for some reason the first option is not available you can try the following steps:
1. Open https://github.com/opennetworkinglab/ngsdn-tutorial and clone the repository using "git clone -b advanced https://github.com/opennetworkinglab/ngsdn-tutorial" (or we will provide the folder- need to check)
2. Manually install or verify the following dependencies:
      Docker v1.13.0+ (with docker-compose)
      make
      Python 3
      Bash-like Unix shell
      Wireshark (optional)
3. If the ngsdn-tutorial directory is already present, make sure to update its content:
      cd ~/ngsdn-tutorial
      git pull origin advanced
    Upgrade the dependencies to the latest version using the following command:
      cd ~/ngsdn-tutorial
      make deps
4. 


