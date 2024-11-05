- Here, Build a docker image using dockerfile it located on my github..First install docker on your machine

      sudo apt-get install docker.io

- Create a new pipeline project

  ![image](Build_docker_image_and_push/Screeshot/1.png)Build_docker_image_and_push/Screeshot

- Add the souce code details of github repository, branch and credentials...

  ![image](./2.png)

- Install a docker_build_step plugin then only you can add the steps on build stage...
  on the build step choose create/build image

  ![image](./5.png)

- Add another build step to push a docker image on dockerhub. Specify the dockerhub url (hub.docker.com)
  Add the dockerhub credentials
   
  ![image](./6.png)

- Build the project...

  ![image](./8.png)
  ![image](./9.png)

> [!IMPORTANT]
> If you face any error like these try to toubleshoot..

![image](./13.png)
![image](./14.png)

> [!TIP]
> Configure these steps

![image](./12.png)

    sudo vim /usr/lib/systemd/system/docker.service

- Add the these line on docker service path file

  ![image](./11.png)

      -H unix:///var/run/docker.sock


> [!TIP]
> If you face permission denied then execute the line
- Then ,Attach the line on jenkins system configuration option

  ![image](./10.png)

      sudo chmod 777 /var/run/docker.sock








