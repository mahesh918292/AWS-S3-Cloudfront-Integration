# AWS-S3-Cloudfront-Integration
![Screenshot (376)](https://github.com/user-attachments/assets/669e4902-5a5e-4802-a650-4ab0341c473d)

Step 1) Create a s3 bucket and upload build
![Screenshot (377)](https://github.com/user-attachments/assets/ba153d04-6d60-4f11-8587-2bb7d6e023d5)
step 2) Go to Properties and Enable static website hosting to serve files to the users.
Specify the root object and error object.
![Screenshot (378)](https://github.com/user-attachments/assets/41f59800-61d0-46b2-ba34-e22a66374b96)
![Screenshot (379)](https://github.com/user-attachments/assets/4749c5a0-06b0-4f72-b7f5-d48898f0035f)
step 3) Block public access so that only cloudfront can be able to communicate with the s3
![Screenshot (380)](https://github.com/user-attachments/assets/5d728ab6-0bb8-4a3e-ad14-7ff5d316157d)
step 4) when the cloudfront is created and attaching s3 automatically policy is attached here in the bucket policy
![Screenshot (381)](https://github.com/user-attachments/assets/d2a03b8e-5669-444e-9bf2-f436a5112157)
step 5) After creating cloudfront this looks like this 
![Screenshot (382)](https://github.com/user-attachments/assets/e6eaba27-104e-4bfb-87e8-9a82d0871cf5)
step 6) Click Edit and put index.html as an entry point 
![Screenshot (383)](https://github.com/user-attachments/assets/47f0e44f-6910-44c3-946c-7bd1f04bf2b4)
![Screenshot (384)](https://github.com/user-attachments/assets/8603027c-2de6-4a33-8639-1fc788ab51b4)
step 7) Result can be seen via cloudfront url
If it shows hit from the cloudfront then it is cahed at edge location , if miss from cloudfront then the files is not cached
