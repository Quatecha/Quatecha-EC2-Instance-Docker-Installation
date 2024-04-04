# EC2 Instance & Docker Installation

## Overview
This guide provides step-by-step instructions for setting up Docker on an Amazon EC2 instance. The project aims to streamline the process of launching an EC2 instance, configuring it, and installing Docker to facilitate application deployment.

## Contributors
- Justin Vargas
- Luis Ventura
- Quatecha Cleveland Webb
- Edgardo Vasquez
- Jose Rodriguez
- D’Andre Walden

## Launching Your EC2 Instance
1. Go to the AWS Management Console and navigate to EC2.
2. Launch a new EC2 instance.
3. Name your instance "ec2-server".
4. Choose Amazon Linux 2 as your AMI.
5. Select the t2.micro instance type.
6. Configure a key pair and download the private key (.pem file).
7. Configure the network settings and security group to allow SSH traffic.
8. Launch the instance.

## How to Install PuTTY
PuTTY is a free and open-source terminal emulator and network file transfer application. Follow these steps to install PuTTY:
1. Download PuTTY from the official website.
2. Install PuTTY on your local machine.
3. Load your private key pair in PuTTYgen.
4. Configure PuTTY settings to connect to your EC2 instance.

## Installing Docker on the EC2 Instance
1. Update the package index by running `sudo yum update -y`.
2. Install Docker using `sudo yum install docker -y`.
3. Start the Docker service with `sudo systemctl start docker`.
4. Verify the installation by running `sudo docker run hello-world`.
5. Enable the Docker service to start automatically with `sudo systemctl enable docker`.
6. Check the Docker version with `docker --version`.
7. Optionally, add your user to the Docker group to run Docker commands without `sudo`.

## Conclusion
Installing Docker on Amazon Linux is a straightforward process that involves a few simple steps. By following this guide, you should be able to set up Docker on your EC2 instance and begin deploying your applications efficiently.

## License
This project is licensed under the [MIT License](LICENSE).
## Presentation
  -https://docs.google.com/presentation/d/1igjwBS6FJP2SoNgHClV-pTZN91uvTj1UGHke5lgAMO0/edit#slide=id.p
