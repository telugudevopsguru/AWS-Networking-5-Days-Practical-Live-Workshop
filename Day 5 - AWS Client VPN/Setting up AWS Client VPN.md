+ <b>Author: Moole Muralidhara Reddy</b></br>
+ <b>Email:</b> telugudevopsguru@gmail.com</br>
+ <b>Website:</b> https://www.telugudevopsguru.com/</br>
+ <b>Mobile:</b>+91 7893121036</br>
+ <b>Description:</b>Setting Up AWS Client VPN endpoint</br>

# Setting  Up AWS Client VPN endpoint :

You can follow the steps below to set up the AWS Client VPN endpoint.</br>
![Lab - Setting up Client VPN endpoint in telugu - Moole Muralidhara Reddy - Telugu Devops Guru](https://github.com/telugudevopsguru/AWS-Networking-5-Days-Practical-Live-Workshop/blob/418192e6fcc3aee122a2c1d0dd5d15356d9f9caf/Day%205%20-%20AWS%20Client%20VPN/Images/Lab%20-%20Setting%20up%20Client%20VPN%20endpoint%20in%20telugu%20-%20Moole%20Muralidhara%20Reddy%20-%20Telugu%20Devops%20Guru.png)

## Step 1: Create the AWS ACM with techworldwithmurali.in

+ Request an SSL/TLS certificate from AWS Certificate Manager (ACM) for the domain "techworldwithmurali.in." This certificate will be used to secure the Client VPN connections.

```xml
 Name: techworldwithmurali.in
```
## Step 2: Create the Active Directory in AWS

Set up an Active Directory (AD) server, either on-premises or in AWS, to manage user authentication for the Client VPN.

```xml
Name: techworldwithmurali.in
```
## Step 3: Create the Client VPN endpoints

Create and Configure the Client VPN endpoints in your AWS environment.
```xml
+ Name: Murali-VPN
+ Client IPv4 CIDR : 10.22.0.0/22

+ DNS server 1 IP address - 10.0.0.2
+ DNS server 1 IP address - 8.8.8.8
```
## 3.1: Target network associations

+ Associate the Client VPN endpoint with the target network(s) that you want to grant VPN access to.
```xml
Add the public subnets to the target network associations.
```
## 3.2: Add the Authorization rules

+ Set up the necessary authorization rules to control which users have access to specific resources through the VPN.
```xml
To allow all users, add the CIDR 10.0.0.0/16.
```
## 3.3: Download the Client Configuration

+ Download the client configuration files for the VPN connection, which will be used to configure VPN client software on the user's devices.

## 3.4: Download the Client VPN software

+ Download and install the appropriate Client VPN software on the user's devices.

## Step 4: Launch the instance in VPC

+ Set up and launch the necessary EC2 instances or resources within your Virtual Private Cloud (VPC) that you want to access through the Client VPN.

## Step 5: Connect the Client VPN and Connect to the private IP's.

+ Connect the VPN client on the user's device to the Client VPN endpoint. Once connected, users will be able to access the private IP addresses of the resources in the VPC.

## Step 6: Congratulations! You have successfully set up the Client VPN endpoints.

+ Confirm that the Client VPN is working correctly, and users can access the intended resources securely.
