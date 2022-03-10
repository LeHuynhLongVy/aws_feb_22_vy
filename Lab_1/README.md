# Lab 1: 

## Long Vy

### IAM USER

#### Create IAM USER

![AWS-IAM-ACCOUNT](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/2-iam-users.png)

![AWS-IAM-ACCOUNT-1](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/iam-vy-1-created-copy.png)

![AWS-IAM-ACCOUNT-2](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/iam-vy-2-created-copy.png)

#### IAM ccount and role's policy
##### Role role-NAME_1 can access all resource of s3 service, but can't access anything of ec2 service.
![policy-1](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/policy-for-iam-user-NAME_1.png)

##### Role role-NAME_1 can access all resource of ec2 service and can do anything of sts (including assume role), but can't access anything of s3 service.
![policy-2](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/policy-for-iam-user-NAME_2.png)

#### Check IAM account permission
![iam-vy-1](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/iam-vy-1-ec2-deny.png)

![iam-vy-1](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/iam-vy-2-s3-deny.png)

#### Create role role-NAME_1 and role-NAME_2

![roles](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/vy-info-role-NAME_1.png)

![roles](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/vy-info-role-NAME_2.png)

#### Trust relationship of role role-NAME_1
##### This mean that role-NAME_1 allows iam account iam-vy-2, role role-NAME_2 and s3 service do assume role itself.
![roles](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/vy-trust-entity-role-NAME_1.png)

### Trust relationship of role role-NAME_2

![roles](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/vy-trust-entity-role-NAME_2.png)

#### Check the result when use assume role for iam-vy-2
##### This is IAM account : iam-vy-2. 
![roles](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/iam-vy-2-result.png)

##### This account can do assume role to role-NAME_1
![roles](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/iam-vy-2-result-2.png)

##### Result of assuming role
![roles](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/iam-vy-2-result-3.png)

### EC2

#### Create Instance EC2

![EC2](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/ec2-t2-micro.png)

![EC2](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/ec2-created-copy.png)

#### SSH to EC2 instance successfully
![ssh](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/vy-ssh-thanh-cong.png)

#### Set role-NAME_2 for ec2 instance
![ssh](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/vy-set-role-name2-cho-ec2.png)

#### Default role of ec2 instance is role-NAME_2 so it can't call AWS S3 LS
![ssh](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/vy-ssh-then-cant-s3.png)

![ssh](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/vy-role-NAME_2-cant-s3-ls.png)

#### Assume role role-NAME_1 for ec2 instance and switch to it
#### Create three environment variables to assume the IAM role role-NAME_1.
![ssh](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/vy-assume-role-and-switch-to-it.png)

#### After that, this ec2 instance can use AWS S3 LS
![ssh](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/vy-aws-s3-ls-ok.png)
