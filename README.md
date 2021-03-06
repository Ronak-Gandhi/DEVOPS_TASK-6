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

![Screenshot (212)_LI](https://user-images.githubusercontent.com/64469896/93686415-b6321380-fad3-11ea-9b7b-621aacc17dd2.jpg)



* **`GROOVY  CODE`** :-

![1](https://user-images.githubusercontent.com/64469896/93686058-5aff2180-fad1-11ea-89ab-576f49b24635.jpg)


~ After running Job-1 , rest other jobs will also creates..

* **`JOB-2`** :-

![Screenshot (220)](https://user-images.githubusercontent.com/64469896/93685967-bc72c080-fad0-11ea-80fe-26f3cce9656f.png)

![Screenshot (221)](https://user-images.githubusercontent.com/64469896/93685970-bed51a80-fad0-11ea-8231-ffbc54191b07.png)


* **`JOB-3`** :-

~ Here i merged job-3(testing) and job-4(email):-

![Screenshot (222)](https://user-images.githubusercontent.com/64469896/93686235-93532f80-fad2-11ea-9e4b-487d62c45d4f.png)

![Screenshot (223)](https://user-images.githubusercontent.com/64469896/93686236-951cf300-fad2-11ea-9ef2-cea39cb79b29.png)

![2](https://user-images.githubusercontent.com/64469896/93686247-9f3ef180-fad2-11ea-8bd0-b59961adb892.jpg)

![Screenshot (225)](https://user-images.githubusercontent.com/64469896/93686252-a665ff80-fad2-11ea-8347-38020e730fbd.png)

**Configuration**:-

![3](https://user-images.githubusercontent.com/64469896/93686253-ab2ab380-fad2-11ea-8026-3b0af3393a08.jpg)


## THANK YOU !!
