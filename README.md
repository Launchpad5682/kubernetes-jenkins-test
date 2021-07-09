## Steps to automate the deployment or any of the Kubernetes Job using Jenkins
* Install kubectl on the Jenkin's node. Then, copy the configuration to the /root/.kube and check the cluster is accessible or not.
* Then, copy the configuration to the Jenkin's user /var/lib/jenkins/.kube.
* After the configuration is complete, now you can easily execute ```kubectl``` commands from the Jenkins execute shell or Jenkinsfile.
* Sometimes, the kubectl command is not accessible then use the full command path like ```/usr/bin/kubectl``` and can also the add the Jenkins user to the sudoers ```/etc/sudoers``` with the line
  ```Jenkins ALL=z(ALL) NOPASSWD:ALL```
```We can use any of the plugin for integrating the Kubernetes but it creates the issues most of the times. So, we should use the basic concepts the rescue```
