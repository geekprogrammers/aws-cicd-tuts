# Creating a pipeline from codecommit repository

---

Whenever we push a change to the master branch of our code commit repo using git push command, our aws code pipeline can be trigerred and it will pull code changes from codecommit repository and deploy it to production s3 bucket.

![image](https://user-images.githubusercontent.com/94220395/141649344-545e0e41-5ccb-4106-9918-e62cf3505b05.png)


**Step1:** - Create a target s3 bucket and enable static website hosting.


**Step2:** - Create pipeline

![image](https://user-images.githubusercontent.com/94220395/141649565-275bff4f-c019-40a0-9a2e-c1c88bcc3330.png)


![image](https://user-images.githubusercontent.com/94220395/141649829-569a8236-7b54-4f7b-a68a-ce7bd3fc8ab0.png)


Skip build step

![image](https://user-images.githubusercontent.com/94220395/141650418-c2105fea-989f-4d90-9ced-b14dfdacffb1.png)

click create pipeline

![image](https://user-images.githubusercontent.com/94220395/141650569-705c0d7d-239c-4421-a5cc-1bace2d76320.png)

**Step3** - If there is any code changes, once we pushed our changes to codecommit repo via git push command, AWS Codepipeline automatically trigerred and deploy the code to target s3 bucket. This is automatic process.
