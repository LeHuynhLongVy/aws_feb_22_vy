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




## Truc

### Tạo IAM User và gán Permission Policy để giới hạn quyền 

##### KITA 1
![KITA1](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/KITA1-1.png)

![KITA1](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/KITA1-2.png)

##### KITA 2
![KITA1](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/KITA2-1.png)

![KITA1](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/KITA2-2.png)

#### Kiểm tra kết quả truy cập service của các User IAM
##### KITA_1 deny EC2 allow S3
![KITA1](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/KITA1-3.png)

![KITA1](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/KITA1-4.png)

##### KITA_2 deny S3 allow EC2 

![KITA1](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/KITA2-3.png)

![KITA1](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/KITA2-4.png)

#### AssumeRole để User KITA_2 được có thể truy cập với quyền của KITA_1 
##### Tạo Policy Assume Role  
![policy](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/policy-assume-role.png)

##### Tạo Role Assume Role 
![policy](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/role-assume-role.png)

#### Gán Policy Assume Role vào IAM User KITA_2 
![policy](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/gan.png)

#### Check lại kết quả
![result](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/check-result.png)

![result](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/check-2.png)

![result](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/check-3.png)

### Tạo EC2 và login SSH 
#### Hiện tại bị báo lỗi không thể launch instance 
![ssh](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/error-a-truc.png)







