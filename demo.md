Jenkins is a Continuous Integration tool that allows continuous development, test and deployment of newly created codes. 

Pipeline: code commit (from development), build, test, release, deploy/deliver(to production)

Architecture: source code repository -> CI server -> build server -> test server -> production server

Master-Slave Architecture: Jenkins master distributes work load to all the slaves

automate anything, web groovy, create jobs and customize all the functionalities

# Node

default: machine

Permanent node and cloud node

cloud node: run docker container, get IP Address, configure clouds, configure templates using docker images

jenkins/agent:alpine-jdk11 (without python), docker-agent-python (with python)

# Item

## free style - execute shell

```bash
echo "Hello World"
ls -ltr
echo 1234 > test.txt
ls -ltr
```

jenkins/agent:alpine-jdk11

## free style - python script

python script from github

poll scm, check every one minute, when there are changes to git repository, build

## pipeline - script

agent, different stages

## pipeline - scm

pipeline script from scm, github, jenkins file, install requirement, run python

blue ocean beautiful ui

