# How To Start Docker Container on PyCharm

1. First go to 
```bash
Preferences -> Project Interpreter 
```
and click on the gear that shows up on the right
now go to 
```bash
Configure Remote Python Interpreter
```
and click the Docker button. Then click your machine name. 

<img src=https://blog.jetbrains.com/wp-content/uploads/2015/12/pycharm-docker_interpreter.png>  />

When you see the dropdown for Images
choose 
```bash
minimum/docker-django-mysite:latest
```
This now generates a docker container that will be used as a project interpreter. 