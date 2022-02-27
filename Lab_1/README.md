# Lab 1: 

## Long Vy


### IAM USER

#### Tạo IAM USER NAME 1 và NAME 2

![AWS-IAM-ACCOUNT](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/2-iam-users.png)

![AWS-IAM-ACCOUNT-1](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/iam-vy-1-created-copy.png)

![AWS-IAM-ACCOUNT-2](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/iam-vy-2-created.png)

#### Policy của NAME 1 và NAME 2

![policy-1](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/policy-for-iam-user-NAME_1.png)

![policy-2](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/policy-for-iam-user-NAME_2.png)

#### Check permission của 2 tk IAM
![iam-vy-1](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/iam-vy-1-ec2-deny.png)

![iam-vy-1](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/iam-vy-2-s3-deny.png)


#### Tạo ROLE NAME 1 và NAME 2

![roles](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/two-roles-2.png)

![roles](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/two-roles.png)
##### Chỉ cần 1 role làm assume role nên chọn role-NAME_1. 
##### Bị sai dòng AWS nên update lại

![roles](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/assume_role_update.png)

#### Kiểm tra kết quả assume role

![roles](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/iam-vy-2-result.png)

![roles](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/iam-vy-2-result-2.png)

![roles](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/iam-vy-2-result-3.png)


### EC2

#### Tạo Instance EC2

![EC2](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/ec2-t2-micro.png)

![EC2](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/ec2-created-copy.png)

#### Copy key file của EC2 sang ubuntu wsl

![wsl](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/lay-ec2-key-file-sang-ubuntu.png)

#### Thử ssh

![ssh](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/key_permission_error.png)

![ssh](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/try-fix.png)

![ssh](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/key_permission_error-not-FIXED.png)

#### Tạo cái ec2 mới với cái phần security là anywhere
![error](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/new_ec2_instance_still_not_work.png)


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
![policy](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/check-result.png)

![policy](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/check-2.png)

![policy](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/check-3.png)

### Tạo EC2 và login SSH 
#### Hiện tại bị báo lỗi không thể launch instance 
![policy](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_1/error-a-truc.png)
