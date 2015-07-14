sonar-vagrantbox
================

* CentOS 6.5 x64
* PostgreSQL
* Sonar 5.1.1

## Usage

    vagrant up

Sonar will be available at http://localhost:9000

To run a php sonar analysis

## Clone a repo into the shared src directory

    cd src
    git clone 'myrepo'

## Set up the sonar project properties (copy the example, then change the project key / name)

    cp src/sonar-project.properties.example myrepo/
    
## Run the project

    vagrant ssh
    cd /var/www/src/myrepo
    /usr/local/sonar-runner/bin/sonar-runner

    
    
