# Lab 3: 

## Long Vy

### Create VPC

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_3.1/1.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_3.1/2.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_3.1/3.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_3.1/4.png)

#### Create 3 public subnets in 3 different AZ

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_3.1/5.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_3.1/6.1.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_3.1/6.2.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_3.1/6.3.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_3.1/6.4.png)

#### Create 3 private subnets in 3 different AZ

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_3.1/7.0.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_3.1/7.1.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_3.1/7.2.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_3.1/7.3.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_3.1/7.4.png)


#### Create 3 database subnets in 3 different AZ

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_3.1/8.0.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_3.1/8.1.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_3.1/8.2.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_3.1/8.3.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_3.1/8.4.png)

#### All subnets

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_3.1/9.png)

#### Create internet gateway

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_3.1/10.0.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_3.1/10.1.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_3.1/10.2.png)

#### Attach igw to vpc

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_3.1/10.3.png)

#### Create Elastic IP address

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_3.1/11.png) 

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_3.1/11.1.png)

#### Create NAT gateway for AZ us-east-1a

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_3.1/11.2.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_3.1/11.3.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_3.1/11.4.png)

#### Steps:

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_3.1/11-all.png)

#### Create NAT gateway for AZ us-east-1b

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_3.1/12-all.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_3.1/12.1.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_3.1/12.3.png)


#### Create NAT gateway for AZ us-east-1c

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_3.1/13-all.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_3.1/13.1.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_3.1/13.2.png)

#### Create route table for the VPC

#### Create route table for public subnet us-east-1a
![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_3.1/14.0.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_3.1/14.1.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_3.1/14.1.1.png)

#### Create route table for private subnet us-east-1a

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_3.1/14.2.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_3.1/14.3.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_3.1/14.4.png)

#### Add route for public us-east-1a rt
![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_3.1/15-create-route-for-public-rt.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_3.1/15.1.png)

#### Add route for private us-east-1a rt
![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_3.1/16-create-route-for-private-rt.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_3.1/16.1.png)



