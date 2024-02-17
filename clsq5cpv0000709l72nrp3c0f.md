---
title: "How to set up theImageGPT project locally"
datePublished: Sat Feb 17 2024 14:01:03 GMT+0000 (Coordinated Universal Time)
cuid: clsq5cpv0000709l72nrp3c0f
slug: how-to-set-up-theimagegpt-project-locally

---

Hey guys, If you are reading this article right now I am glad you took an interest in trying out my small project.

For the first step fork and clone the GitHub repository:

```plaintext
https://github.com/<your github username>/theImageGpt
```

Navigate to the project folder

```plaintext
cd theImageGpt
```

Then install the required packages using npm by running the following command

```plaintext
npm i
```

Now create the ***.env*** file

```plaintext
cp .env.sample .env
```

We have used several environment variables, most of which are from different external sources. This project has been made using openai API. So first you need to create an account in [openai](https://platform.openai.com) and retrieve your API key.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1708013596009/47da6e98-2660-4220-9f57-d82615048463.png align="center")

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1708013613243/7cb98b84-fc7d-43b7-b2dc-5fec8a53fedf.png align="center")

Copy the key and paste it into the .env file.

Now we need to set up the database to store the API limit of the user. In this project when a new user creates an account they get 5 free credits to generate images where 1 image generation costs 1 credit. So we need to store and count the credits for each user. In this project, we have used a Postgres database from planetscale.

***Note:***

When I created this project planetscale had a free tier plan in India, but currently, they are not offering the free plan in India.

If you are from any other place and have access to the free plan, you can follow the tutorial further.

Visit the planetscale website and create an account, then click Create a new database.

Give a database name and then leave everything as default, then click on Create.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1708102552204/405852ab-2ba2-4ec2-9e3b-594c4fa8647f.png align="center")

Select Prisma here cause we are going to use this for the project.

Now create a password below

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1708102671238/8d8f6290-fe15-4b1b-8f8a-f0669a0c3074.png align="center")

After that below you would get the database URL which you need to copy and put into the .env file.

Now, the database part has been completed. We need to set up the authentication now.

We have used clerk authentication in this project. Visit the [Clerk](https://clerk.com) website and then create an account. Click on Create New Application then give the application name and select Google Authentication. You can choose which ones you want.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1708104968150/7a2a857c-efb8-45e6-b5b3-e50622b276b8.png align="center")

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1708104980417/7b86f8ab-1510-492e-ab4c-029f44ab0551.png align="center")

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1708105039607/720627a7-84cb-4bb4-ab9f-c574d1b66b27.png align="center")

Now copy both these keys and paste them into the .env file.

Now all the steps have been completed. Go the terminal and run the following command.

```plaintext
npm run dev
```

Now visit localhost and the website would be running fine.