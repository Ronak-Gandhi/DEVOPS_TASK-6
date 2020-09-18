# DEVOPS_TASK-6

## TASK OBJECTIVE:-

_Perform third task with the help of Jenkins coding(groovy) file ( called as Jenkins file approach ) and perform the with following phases_:

`1.` **Create container image that’s has Jenkins installed using dockerfile Or You can use the Jenkins Server on RHEL 8/7**.

`2.` **When we launch this image, it should automatically starts Jenkins service in the container**.

`3.` **Create a job chain of job1, job2, job3 and job4 using build pipeline plugin in Jenkins**.

`4.` **`Job2 ( Seed Job )`** :  *  _**Pull the Github repo automatically when some developers push repo to Github**_!

`5.` **Further on jobs should be pipeline using written code using Groovy language by the developer**.

`6.` **`Job1`**:

  * _**By looking at the code or program file, Jenkins should automatically start the respective language interpreter installed image container to deploy code on top of Kubernetes ( eg. If code is of PHP, then Jenkins should start the container that has PHP already installed )**_!

  * _**Expose your pod so that testing team could perform the testing on the pod**_!

  * _**Make the data to remain persistent using PVC ( If server collects some data like logs,other user information )!
  
 `7.` **`Job3`** : _**Test your app if it is working or not**_!
  
 `8.` **`Job4`** : _**if app is not working , then send email to developer with error messages and redeploy the application after code is being edited by the developer**_!
