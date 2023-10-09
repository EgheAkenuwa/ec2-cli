# ec2-cli
## STEP 1
– Configure AWS Credentials, using the “aws configure” command and then proceeding to supply the “Access Key ID and Secret Access Key ID” as well as the region Region name of the AWS and default format.
![image](https://github.com/EgheAkenuwa/ec2-cli/assets/144701841/5c793a47-1fab-4250-81cc-cb0c1613b865)
## Step 2 
- Create Key Pair
![image](https://github.com/EgheAkenuwa/ec2-cli/assets/144701841/c58ffe3c-89fc-4cb8-bc20-891ad75cb3a4)
## Step 3
- Describe Key Pairs with the command aws ec2 describe-key-pairs
  ![image](https://github.com/EgheAkenuwa/ec2-cli/assets/144701841/36f9008f-562e-4e07-b3c4-726ef935b9cd)
  ## Step 4
  -- CREATE SECURITY GROUP
  -- First Check Ip address using checkip.amazonaws.com
  ![image](https://github.com/EgheAkenuwa/ec2-cli/assets/144701841/d15a5d07-07d5-4383-bc87-d88cf7473991)

  --Create the  Security group using aws ec2 authorize-security-group-ingress –group-id (security  group id) –protocol tcp –port 22 –cidr(ip adresss got earlier)
  ![image](https://github.com/EgheAkenuwa/ec2-cli/assets/144701841/2c19eea6-b992-4755-93df-a911023f9684)

-- Step 5 Create EC2 Instance
![image](https://github.com/EgheAkenuwa/ec2-cli/assets/144701841/799ebf1a-52fd-413f-85a3-fad38491d63e)
## step 6
-- CONFIRM THE INSTANCE
![image](https://github.com/EgheAkenuwa/ec2-cli/assets/144701841/107690e8-154d-4ba9-aed8-3272518fabfa)

## We have successfully created and ran and EC2 Instance using CLI
## Step 7
-- TERMINATING INSTANCES
use the command aws ec2 terminate-instances instance-id
![image](https://github.com/EgheAkenuwa/ec2-cli/assets/144701841/0cb92cdc-1c1d-4670-99d8-7f12b03e1cf7)

-- Confirm the Instance is terminated
![image](https://github.com/EgheAkenuwa/ec2-cli/assets/144701841/c7a2dfff-0565-4e3e-831c-9bb7ea580605)

--DELETE KEY PAIR USING THE COMMAND aws ec2 delete-key-pair –keyname (name of key)
![image](https://github.com/EgheAkenuwa/ec2-cli/assets/144701841/ccca5ad8-1dbe-40f0-8971-f295305df0aa)


-- DELETE SECURITY GROUPS by the command aws ec2 delete-security-group –group-name (name of group)

![image](https://github.com/EgheAkenuwa/ec2-cli/assets/144701841/18fef5b5-ad38-47da-9a67-adf21e8fe849)











