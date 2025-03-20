Documentation of the base image : https://hub.docker.com/r/jenkins/inbound-agent

docker build . -t jenkins_agent_symfony

docker run --name jenkins_agent_symfony_container --init jenkins_agent_symfony -url http://172.17.0.2:8080 223d0e75ef8907a3625219b939be746204c55509ea1ee495702226c9e3d366d4 JenkinsAgent_composer

To get the <IPAdresse_of_jenkins_master>, make this command :
docker inspect jenkins_master_container

<password> and <node_name> are given by the jenkins_master when you create a node