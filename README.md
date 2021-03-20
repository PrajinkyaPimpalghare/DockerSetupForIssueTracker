# DockerSetupForIssueTracker
Its Docker Container setup for IssueTracker Django project. IssueTracker website docker image get created from Docker Python 3.7 base image and on the top of it seeting of modules and running of the server in container enviroment takes place.[In windows]

# Summary: 
  Base Django project is present in git@github.com:PrajinkyaPimpalghare/IssueTracker.git , this project has been moved to container enviroment.
  Prerequisties: Docker installed on windows.
  Steps For Image Creation :
  mkdir DockerProject
  Copy Django project in it 
  Update Setting.py with static files path
  in Dockerproject folder update the Dockerfile
  
  Commands: 
  docker build -t issue-tracker-in-docker .
  docker run -it -p 8020:8020 issue-tracker-in-docker
  
  Access website at :  http://localhost:8020 or http://127.0.0.1:8020/
  If private IP is available, update that ip in setting.py allowed host section.
  
  Thats it, like this you can containerize any application and enable its networking.
