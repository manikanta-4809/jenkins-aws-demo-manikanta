# explanation
### Goal:To build a fully automated CI/CD system that takes code from a developer's machine, builds it, tests it, packages it, and deploys it to the cloud.

In this we need to run the jenkins pipeline succesfully and build to be sucess.First we need to create two ec2 instances using terraform provider and name them as jenkins-master and jenkins-agent.in master we need to give inbound rules as ssh,http,https and custom tcp as 8080 . 8080 is used for run jenkins.and for agent we only allow ssh.
after this we need to ssh both the master and agent using their ip address in two different terminals.in these we can use linux or ubuntu but i used ubuntu for easy way.after doing ssh we need to install jenkins to access and also we need to install nodejs because we are building using nodejs application.and also insatll docker.after this we need to get public key and private key of agent ,we are having commands to use it.and after that public key of agent in master using echo command.after this we need to run the public ip of master with port 8080 there we can see jenkins start.then using that we need to install recommended plugins.after login we need to create a credientials and after that we need to create a node and name it label as ubuntu.we need to create a repository in github and push the app.js and package.json files and after that we need to add a file jenkins in it.after this we need to build a pipeline using the created repostiory and after that we need to build it we can see the output as successful.


### deliverables

![Screenshot (140)](https://github.com/user-attachments/assets/675d2c69-df0d-46bd-a416-4e356335eab0)

![Screenshot (141)](https://github.com/user-attachments/assets/cb8b09ac-fd26-4bf4-bf63-f4c8c3ad5e30)

![Screenshot (142)](https://github.com/user-attachments/assets/b2f5ae68-ee29-4d37-b1ec-6491ecbdd930)

agent
![Screenshot (143)](https://github.com/user-attachments/assets/4d3065c3-bd97-46a8-bd05-b732e06f03fd)

master
![Screenshot (144)](https://github.com/user-attachments/assets/cece43ab-68fc-40e4-8625-417de621465a)





