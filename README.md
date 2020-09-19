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

  * _**Make the data to remain persistent using PVC ( If server collects some data like logs,other user information )**_!
  
 `7.` **`Job3`** : _**Test your app if it is working or not**_!
  
 `8.` **`Job4`** : _**if app is not working , then send email to developer with error messages and redeploy the application after code is being edited by the developer**_!

---

* **`DOCKERFILE`**:-

![Screenshot (207)](https://user-images.githubusercontent.com/64469896/93621285-f53f6680-f9f8-11ea-82ae-32b41d3a2705.png)


* _To use Groovy code,we have to download a plugin ,called **`Job DSL`** !!_

![Screenshot (205)](https://user-images.githubusercontent.com/64469896/93670738-31d39680-fabb-11ea-83a3-e2d4658734c3.png)

~ To use the Job DSL plugin, you first need to create a seed job. The seed job is a Jenkins job which runs a DSL scripts, and then generates a new job. The seed job is a normal free-style Jenkins job that you add the “Process Job DSL” build step. This step takes the DSL and generates the configured jobs.


* **`JOB-1`** :-

![Screenshot (208)](https://user-images.githubusercontent.com/64469896/93670730-284a2e80-fabb-11ea-8a45-c8abbe003ff4.png)

![Screenshot (209)](https://user-images.githubusercontent.com/64469896/93670735-3009d300-fabb-11ea-9743-85f8a9948d8e.png)

![Screenshot (210)](https://user-images.githubusercontent.com/64469896/93670736-313b0000-fabb-11ea-83a0-c6a8f6e150a9.png)

![Screenshot (211)](https://user-images.githubusercontent.com/64469896/93670809-baeacd80-fabb-11ea-95bf-f6358e1ccbd1.png)


* **`GROOVY  CODE`** :-

![InkedScreenshot (219)_LI](https://user-images.github usercontent.com/64469896/93671002-18334e80-fabd-11ea-83c3-b9435e82ab5a.jpg)

~ After running Job-1 , rest other jobs will also creates..

* **`JOB-2`** :-





