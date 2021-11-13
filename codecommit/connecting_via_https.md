
**Step1:** - Create IAM user with required permission and we cannot perform Codecommit activities with root user.

**Step2:**- we have to create new user with required permission. After new user created attach AWSCodeCommitPowerUser policy to that and generate HTTPS git cred.

https://docs.aws.amazon.com/codecommit/latest/userguide/setting-up-gc.html?icmpid=docs_acc_console_connect_np

![image](https://user-images.githubusercontent.com/94220395/141646370-73ed0445-39d3-409d-985b-f41da891de8b.png)

**Step3:** - 
In locally execute

git init 

git remote add origin {GIT CLONE PATH}

**then git add and do commit then git push changes**
