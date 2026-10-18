| Deployment | Public IPv4 address | Connection method | Screenshot | Instance terminated? |
|------------|---------------------|-------------------|------------|----------------------|
| 1 | 13.59.124.109 | EC2 Connect / SSH | screenshots/deployment-1.png | Yes |
| 2 | 3.150.127.61 | EC2 Connect / SSH | screenshots/deployment-2.png | Yes |
| 3 | 3.16.157.141 | EC2 Connect / SSH | screenshots/deployment-3.png | Yes |


## Deployment 1 – small
1. Launch instance from template
2. Select small free Instance type
3. Confirm User Data in Advanced Details
4. Launch instance
5. Open Link
6. Connect
   - Wait for Status to pass checks
   - Connect
   - 1.9Gi memory
   - Default port 22 SSH from Security Group
7. Screenshot
## Terminate EC2 – Deployment 1
1. EC2 > Instances (running) > Instance State > Delete

## Deployment 2 – micro
1.	Launch instance from template
2.	Select small free Instance type
3.	Confirm User Data in Advanced Details
4.	Launch instance
5.	Open Link
6.	Connect 
    -	Wait for Status to pass checks
    -	Connect 
    -	913 Mi memory
    -	Default port 22 SSH from Security Group
7.	Screenshot 
## Terminate EC2 – Deployment 2
1.	EC2 > Instances (running) > Instance State > Delete

## Deployment 3 – large
1.	Launch instance from template
2.	Select large free Instance type
3.	Confirm User Data in Advanced Details
4.	Launch instance
5.	Open Link
6.	Connect 
     -	Wait for Status to pass checks
     -	Connect 
     -	3.7Gi memory
     -	Default port 22 SSH from Security Group
7.	Screenshot 
## Terminate EC2 – Deployment 3
1.	EC2 > Instances (running) > Instance State > Delete

## Summary
CPU is usage, but all three were 0% with 2 vCPUs. Each free tier size has different memory sizes. All three had the same size disk and usage amount. Uptime was how long the instance was running. 

Each instance further helped me recall the process from Class 6. No errors were encountered other than removing the cobwebs from my memory. I don’t see any instances running but I do see the launch template still available. 
