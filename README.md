# technical_solutions
This include technical solutions using terminal commands from Linux and Mac OS 




How to delete panopto_upload from your Mac laptops/Mac Desktop?




Panopto creates a user account in your system and locks it with a random password so you cannot log in and access it.

Its a background process that has created an account so you cannot access it using Settings/System Preferences. In order to remove it, follow the steps as shown below:

 

Step 1:

dscl . -list /Users

Step2:

dscl . -read /Users/panopto_upload

Step3:

sudo dscl . -delete /Users/panopto_upload
