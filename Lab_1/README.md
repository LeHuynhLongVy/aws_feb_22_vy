# Lab 1: 

## Long Vy

### IAM USER

#### Create IAM USER

![AWS-IAM-ACCOUNT](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/2-iam-users.png)

![AWS-IAM-ACCOUNT-1](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/iam-vy-1-created-copy.png)

![AWS-IAM-ACCOUNT-2](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/iam-vy-2-created-copy.png)

#### IAM ccount and role's policy

![policy-1](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/policy-for-iam-user-NAME_1.png)

![policy-2](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/policy-for-iam-user-NAME_2.png)

#### IAM account and role's permission
![iam-vy-1](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/iam-vy-1-ec2-deny.png)

![iam-vy-1](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/iam-vy-2-s3-deny.png)


#### Create role role-NAME_1 and role-NAME_2

![roles](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/vy-info-role-NAME_1.png)

![roles](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/vy-info-role-NAME_2.png)

#### Trust relationship of role role-NAME_1

![roles](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/vy-trust-entity-role-NAME_1.png)

### Trust relationship of role role-NAME_2

![roles](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/vy-trust-entity-role-NAME_2.png)

#### Check the result when use assume role for iam-vy-2

![roles](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/iam-vy-2-result.png)

![roles](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/iam-vy-2-result-2.png)

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
![ssh](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/vy-assume-role-and-switch-to-it.png)

#### AWS S3 LS ok
![ssh](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/vy-aws-s3-ls-ok.png)
