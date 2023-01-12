# NetCache_2023
Electrical and Computers engineering - 4th year project

Update Background

Setting the enviroment:
option 1 - Recommended
1. Open https://github.com/opennetworkinglab/ngsdn-tutorial and clone the repository using "git clone -b advanced https://github.com/opennetworkinglab/ngsdn-tutorial".
2. Follow the installation guide in the Readme, use "Option 2 - Manually install Docker and other dependencies".
3. This tutorial contains several exercice, some of the are irrelavant to our project.
   Yet, in order to make sure that the setup of the enviroment will work we suggest coping all the files in the "solutions" repository to the                corresponding place in the main repository "ngsdn-tutorial".
   In addition, we highly recommend following the steps in Exercise 7 in order to gain a deeper understanding of the process.
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
4. In order to start the enviroment follow the next steps:
   1. Open the terminal cd into the ngsdn-tutorial respository
   2. Start the containers by running "sudo start-v4"
   3. Wait about 1 minute before proceeding with the next steps. This will give ONOS time to start all of its subsystems.
   4. Open up the ONOS CLI by running "sudo onos-cli", the password is "rocks".
   5. Activate the fabric and segmentrouting applications by runnig this command in the onos cli: "app activate fabric" , "app activate segmentrouting".
   6. Verify that thos applications have been activated by running this command in the onos cli: "apps -s -a". There should be 21 activate applications.
   7. Run the following commands in the onos-cli: "cfg set org.onosproject.net.flow.impl.FlowRuleManager fallbackFlowPollFrequency 4"
                                                  "cfg set org.onosproject.net.group.impl.GroupManager fallbackGroupPollFrequency 3"
   8. Open up the Mininet CLI in another teminal by using "make mn-cli" in order to test connectivity. try a few pings.

