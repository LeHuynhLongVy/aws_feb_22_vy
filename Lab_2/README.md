# Lab 2: 

## Long Vy

### IAM USER

#### Create an EC2 instance with type t2.micro ( in a public subnet )

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/1-t2-micro.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/1-t2-gp3.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/1-t2-micro-subnet.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/2-t2-use-same-lab2-key.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/3-ec2-created.png)

#### Connect SSH to the EC2 instace
![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/4-1-ssh-to-lostssh-successfully.png)

#### Remove authorized_key folder and disconnect
![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/4-2-remove-authorized_keys.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/4-3-cant-ssh.png)

#### Restore the authorized_keys to retore SSH access
![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/5-check-volume-id-lostssh.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/5-stop-lostssh-instance.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/6-search-for-lostssh-volume-and-detach.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/7-successfully-detached-volume.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/8-attach-the-lostssh-volume-to-recoverssh-instance.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/8-successful-attach-the-lostssh-volume-to-recoverssh-instance.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/9-ssh-to-recoverssh.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/10-mount-xvdp1-to-tmp-folder.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/11-check-ssh-in-recoverssh-instnace.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/11-check-ssh-in-the-mounted-volume.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/12-copy-authorized-to-lostssh-volume.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/15-stop-recover.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/16-detach-lostssh-vol.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/17-reattach-lotssh-vol-to-lostssh-instance)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/18-successfull-reattach.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/19-start-lostssh-again.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/20-ssh-to-lostssh-sucessfully.png)

#### Not using SSH, connect to the EC2 instance by Session Manager
![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/21-create-new-role.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/22-new-role-policy.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/23-new-role-created.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/24-attach-new-role-to-lost-ssh.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/25-succesfully-attach-new-role-to-lost-ssh.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/26-go-to-sm-and-connect.png)

#### Install nginx on the EC2 instance not using docker
![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/27-install-nginx.png)

#### Configure EC2 instance can be accessed HTTP 80 from the Internet
![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/28-configure-nginx.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/29-add-more-network-security-to-be-able-to-access-from-anyip.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/30-check-for-the-ip.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/31-successfully-view-the-html-file.png)

#### Sending nginx access logs to CloudWatch
![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/32-add-full-access-cloudwatch.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/33-install-awslogs-service.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/34-create-config-file-for-awslogs.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/35-config-file-content.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/36-logs-group-on-cloudwatch.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/37-access-and-error-log-stream-of-nginx.png)

#### Create S3 bucket
![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/39-create-s3-bucket.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/40-s3-bucket-created.png)

##### EC2 add policy S3fulladmin
![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/41-add-full-access-s3.png)

##### conjob update every 1 hour
![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/42-1-check-html-folder.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/43-shell-file-to-do-aws-s3-sync.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/44-test-some-function.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/45-test-result.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/46-1-create-a-cron-job.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/46-2-create-a-cron-job.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/48-cronjob-sync-successfully.png)

#### Create a CloudWatch dashboard:

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/49-create-dashboard.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/50-download-clouwatch-agent.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/51-add-cw-agent-server-policy.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/52-add-logs-policy.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/54-run-wizard.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/53.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/55-install-required-package.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/56-install-require-package.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/57-get-mem.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/58-check-cloudwatch.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/59-result.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/60-result.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/61-create-log-filter.png)

![image](https://github.com/LeHuynhLongVy/aws_feb_22_vy/blob/main/Lab_2/62-done.png)


