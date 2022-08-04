
# Software Questionnaire

A static webpage that gathers information from undergraduates on 
their knowledge of programming languages and framework technologies.

## Features
- Uses bright green CSS styling to improve user perception and experience.
- Packaged a Dockerfile with Apache HTTP Server and created a Docker image to deploy on Amazon Elastic Container Registry and Microsoft Azure Container Registry.

## Demo

Insert gif or link to demo
<video width="320" height="240" controls>
  <source src="https://user-images.githubusercontent.com/86692163/182771971-7cc08d20-030e-4550-a3d0-13ac1594af6d.mp4" type="video/mp4">

Your browser does not support the video tag.
</video>

## Lessons Learned

The 1st challenge I came across was not having Docker commands installed on my Amazon EC2 Linux instance.
I overcame this challenge by searching on Stack Overflow and found the solution was to install Docker using sudo commands.

    1. Update the packages on your instance

    [ec2-user ~]$ sudo yum update -y

    2. Install Docker

    [ec2-user ~]$ sudo yum install docker -y

    3. Start the Docker Service

    [ec2-user ~]$ sudo service docker start

The 2nd challenge I came across was understanding how to package a webpage with Docker.
I overcame this challenge by learning how to create a Dockerfile and packaging it with Apache HTTP Server.

    FROM httpd
    COPY . /usr/local/apache2/htdocs/

The 3rd challenge I came across was after having a successful deployment on Amazon Elastic Container Registry, only the default Apache HTML page is displayed.
I haven't overcome this challenge yet, but I believe it must be a directory pathing error.

In this project, I learned how to overcome creating docker image and docker deployment issues.
In addition, I improved my knowledge of HTML, CSS, Docker.

## Screenshots

![App Screenshot](https://via.placeholder.com/468x300?text=App+Screenshot+Here)

