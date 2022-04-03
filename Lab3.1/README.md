# Lab 3: 

## Long Vy
### Task 1
### Create VPC

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/1.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/2.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/3.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/4.png)

#### Create 3 public subnets in 3 different AZ

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/5.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/6.1.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/6.2.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/6.3.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/6.4.png)

#### Create 3 private subnets in 3 different AZ

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/7.0.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/7.1.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/7.2.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/7.3.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/7.4.png)


#### Create 3 database subnets in 3 different AZ

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/8.0.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/8.1.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/8.2.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/8.3.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/8.4.png)

#### All subnets

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/9.png)

#### Create internet gateway

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/10.0.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/10.1.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/10.2.png)

#### Attach igw to vpc

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/10.3.png)

#### Create Elastic IP address

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/11.0.png) 

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/11.1.png)

#### Create NAT gateway for AZ us-east-1a

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/11.2.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/11.3.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/11.4.png)

#### Steps:

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/11-all.png)

#### Create NAT gateway for AZ us-east-1b

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/12-all.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/12.1.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/12.3.png)


#### Create NAT gateway for AZ us-east-1c

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/13-all.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/13.1.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/13.2.png)

#### Create route table for the VPC

#### Create route table for public subnet us-east-1a
![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/14.0.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/14.1.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/14.1.1.png)


#### Create route table for private subnet us-east-1a

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/14.2.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/14.3.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/14.4.png)

#### Create route table for public/private subnet us-east-1b/1c

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/14.5-create-rt-for-the-others.png)

#### Add route for public us-east-1a rt
![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/15-create-route-for-public-rt.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/15.1.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/17.png)

#### Add route for public us-east-1b/1c rt
![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/15-create-route-for-public-1b-1c.png)


#### Add route for private us-east-1a rt
![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/16-create-route-for-private-rt.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/16.1.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/17.1.png)

#### Add route for private us-east-1b/1c rt
![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/16-create-route-for-private-1b-1c.png)

#### Associate public rt to public subnet
![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/18.0-associate-public-rt-to-public-subnet.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/18.0.1.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/18.1.png)

#### Associate private rt to private subnet
![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/19.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/19.0.1.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/19.1.png)

### Task 2,3
#### Create security group that allow ssh port 22 and tcp port 80
![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/20.0.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/20.4.png)

#### Create EC2
#### EC2 in public subnet us1a with public ip
![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/21-ec2-public-1a.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/21.1.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/21.1.1.png)

#### EC2 in public subnet us1b with public ip
![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/22-ec2-public-1b.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/22.1.png)

#### EC2 in private subnet us1a

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/23-ec2-private-1a.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/23.1.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/24.png)


#### SSH to EC2 in subnet public_us_1a and then ssh to EC2 in subnet private_us_1a and ping google

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/25.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab3.1/25.1.png)

#### Task 4