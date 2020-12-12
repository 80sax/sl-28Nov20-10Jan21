CI CD Using Jenkins

## Agenda

    Introduction
    Concepts
        - Continuous Integration
        - Continuous Delivery
        - Continuous Deployemnt
    Jenkisn installation and configuration
    Plugins
    Sample Jobs
    Upstream/Downstream Projects
    Parameterized Builds
    Build triggers
    Distributed Builds (Jenkins Build Slaves)

    Jenkins Pipelines (Pipeline-as-Code)


## Installationa and Configuration


access the server on the browser:

localhost:8080
127.0.0.1:8080
<IPaddress>:8080



Build Tools
    - Java
        - Ant (Build.xml)
        - Maven (POM.xml)
        - Gradle (build.xml)
    .Net
        - MSBuild (Build)
        - Octopus Deploy (Deployment Automation)
    

Buildtool - Maven
Environment - JDK
Build triggers
    Poll SCM

Plugins


https://github.com/sk12k/addressbook

mvn -f pom.xml package

Classroom Exercise

1. Source Code: https://github.com/sk12k/addressbook.git

2. Build Step: Maven
    - Goal: package
    - POM: pom.xml


test ----> Staging ----> deploy

Project
    - JobA
        - Build#1
        - Build#2
    - JobB
        - Build#1
        - Build#2


This project will deploy the artifact in Test Environment on App Nodes
This project will deploy the artifact in prod Environment on DB Nodes

http://209.97.128.222:8080/job/deploy/configure

curl -u admin:passw0rd http://209.97.128.222:8080/job/deploy/build?token=mysupersecureauth


Build Nodes
    - Maven
        - host1
        - host2
        - host3
    
    - .Net
        - winhost1
        - winhost2
        - winhost3
    
    - Pythonslaves
        - host4
        - host5
        - host6

## Post Commit Hooks

yourrepo/.git/hooks/post-commit

#!/bin/sh
curl -u admin:passw0rd http://209.97.128.222:8080/job/deploy/build?token=mysupersecureauth

Note: make sure the "post-commit" file is executable



## Assignements:

    1. Practice Additional Git Concepts

        git tag         - https://git-scm.com/book/en/v2/Git-Basics-Tagging
        git blame       - https://www.atlassian.com/git/tutorials/inspecting-a-repository/git-blame
        git stash       - https://git-scm.com/book/en/v2/Git-Tools-Stashing-and-Cleaning
        git rebase      - https://git-scm.com/book/en/v2/Git-Branching-Rebasing
        git cherry-pick - https://www.atlassian.com/git/tutorials/cherry-pick


    2. Configure Webhook in GitHub (in your own repo)

    3. Teamcity installation
    Simplilearn LMS --> Self Learning --> Video 4.7

    4. Lesson End Exercise (Email extension plugin in Jenkins)


## References:
    https://www.martinfowler.com/articles/continuousIntegration.html
    https://www.thoughtworks.com/continuous-integration
    https://d1.awsstatic.com/whitepapers/overview-of-deployment-options-on-aws.pdf
    https://www.jenkins.io/
    Jenkins on MacOS: https://coralogix.com/log-analytics-blog/how-to-install-and-configure-jenkins-on-the-mac-os/
    Maven Documentation: https://maven.apache.org/guides/introduction/introduction-to-the-lifecycle.html
    https://d1.awsstatic.com/Projects/P5505030/aws-project_Jenkins-build-server.pdf
    


