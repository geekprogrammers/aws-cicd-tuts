# aws-codecommit-hints

Aws Code pipeline supports code commit repository which is AWS private repo, Github and Bitbucket(Currently In beta stage)

![image](https://user-images.githubusercontent.com/94220395/141641725-fc1209db-fea0-40be-a69e-7863799da731.png)


**What is code commit ?**

AWS CodeCommit is a version control service hosted by Amazon Web Services that you can use to privately store and manage assets (such as documents, source code, and binary files) in the cloud. For information about pricing for CodeCommit.

Code Commit Can integrated with various AWS service like **AWS Cloudformation, AWS Elastic Beanstalk, Lambda, SNS, Monitor your repo using cloudwatch events**

![image](https://user-images.githubusercontent.com/94220395/141641061-6eabf297-2da4-44f0-b941-ee7108b1cbda.png)

we can intergrate AWS Codebuild directly with AWS Codecommit so when you run you project, codebuild directly pull your code from codecommit repository.

![image](https://user-images.githubusercontent.com/94220395/141640009-e5caa186-6618-4251-a6c0-807d7182cfe4.png)

We can create pipeline on AWS using AWS CodePipeline starting from CodeCommit repository.
**->** So once we pulled code from AWS Codecommit repository our AWS pipeline can build our code using AWS Codebuild and it will deploy it by using one of the code providers suggest it AWS code Deploy.

![image](https://user-images.githubusercontent.com/94220395/141642957-bcd682df-3886-4bd6-8897-9f7c4a791ff0.png)

Data in code commit by default is encrypted by default KMS key 

**Creating Code Commit** -- Basicsally it's repo creation to push and pull with different branches to manage it as like git

![image](https://user-images.githubusercontent.com/94220395/141643626-28f489b9-94a1-4f4f-88e9-239dbdb75be4.png)

Once it's created, in cosole we can see different methods to access it like HTTPS, SSL and HTTPS(GRC)

![image](https://user-images.githubusercontent.com/94220395/141643690-d6ed998a-ece9-4555-a02b-f83377631e0f.png)
