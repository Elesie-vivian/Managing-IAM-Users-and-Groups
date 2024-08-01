# Managing-IAM-Users-and-Groups

## Objective

This Project explores creating and Managing IAM Users and Groups in AWS.
The aim is to demonstrate how to enhance secure access using IAM and Policies for Users and Groups and how Policies determine the extent of permission an IAM User has in an WAS resource.

### Creating Users

I set up an IAM user called Dolly,configuring access types and permissions. 

![alt text](<Images/Image 1.PNG>)

### Creating IAM Groups

I created a group called D-Engineer and assigned permissions to define the Group Policies.

![alt text](<Images/Image 2.PNG>)

### Assigned IAM_VIEW_ONLY 

Here, we assigned the user Read Only permissions on IAM, attached the “IAM_View_Only” Policy to User (Dolly).

![alt text](<Images/Image 3.PNG>)

### Testing Assigned IAM_VIEW_ONLY Permissions

We proceeded to test the attached Permission logging in as Dolly with the log in credentials.
Attempts to access resources on IAM returned “Access Denied to perform function. No identity-based policy allows the action”.
However, I am able to read resources on IAM but can’t perform any additional actions.
This further demonstrates the role played by IAM in ensuring security of resources on AWS as it showcases how permissions define the actions performed by a user.
