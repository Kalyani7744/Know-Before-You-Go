# Azure Immersion Workshop: Cloud Native Apps

Instructor should make sure that the attendees follow the **lab guide** provided in the environment to perform the lab instead of lab guide from MCW repo. Because few instructions may differ from the provided lab guide and MCW repo lab guide. 

### Known Issues and workarounds
- [Know issues in Lab Steps](#know-issues-in-lab-steps)
- [Copy paste issue](https://docs.cloudlabs.ai/Learner/Troubleshooting/CopyPaste)
- [Lab VM connectivity issue](https://docs.cloudlabs.ai/Learner/Troubleshooting/RDP)

#### Know issues in Lab Steps

1. Attendees should make sure that they will go through every instruction properly while performing the before hands-on-lab. If at all the lab guide is not followed correctly, attendees will be facing issues in next part of the lab due to the dependency.

1. The Azure cloud shell can be unresponsive at times; we would suggest you to restart the cloudshell and try again.

1. **Yaml files**:
   While **editing or inserting** the content into the yaml files, attendees should make sure they read the instructions properly and edit the files accordingly. It is better to cross check the files once, after editing and before saving them. 

1. If attendee’s session to build-agent vm gets disconnected,  

   To reconnect to the vm, follow the instruction provided in the before hands-on-lab. 

   - From Environment details page go to **Command to Connect to Build Agent VM** copy the ssh key and paste in cloud shell. 
   - In the cloud shell output, paste the ssh key that you copied earlier enter **yes** when prompted. 
   - Enter the Buid Agent VM password provided in environment details, you will be connected to Build Agent VM. 

1. If attendees are having trouble exiting the `Vim` session with esc, try using `ctrl+ [`  to exit the session. 

1. Issues in before hands-on-lab task 6 due to unsuccessful cloning of **Fabmedical** repo. 

    - Ask attendee to verify that whether he had cloned the **Fabmedical** repository properly. If   not, ask the attendee to run the command,  **git clone <GITHUB\_REPOSITORY\_URL>** to clone the **Fabmedical** repo and perform the step again.    
    
1. Issue in Exercise 1 Task 2 Step 4 

   When adding migration project if attendee gets the error the connection timed out. Possible reasons for this include 

     - The address and/or port was not correct, or the server is not running, it's a temporary issue and wait for 5-10 minutes then retry again.
     - The mongodb might not be running, run the following command on the build VM to start the DB.
       
       ```docker container start mongo``` 

1. Azure API issue: 

     - Due to recent changes in Azure APIs , They are taking additional time to fetch the details of the resources. The validation steps might fail initially for the lab, if you re-run the steps again after 30-45 minutes later then it will succeed if there will be no configuration related issue with lab steps you performed.