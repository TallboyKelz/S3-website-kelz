<img width="1385" alt="Screenshot 2024-05-21 at 2 55 40 PM" src="https://github.com/TallboyKelz/S3-website-kelz/assets/133192420/6e883658-f27a-4120-a805-e21977d588b3"># Overview
This documentation will provide an overview of hosting a static website using AWS's S3. 

# Prerequisites
* An AWS account
* Basic knowledge of the AWS S3 Service
* HTML, CSS, Javascript

# Tools Used
* **AWS S3**: For holding the objects (files) of the website.
* **Text Editor**: For creating or editing the website files. Vscode will be used for this documentation.
  
# Setting up the AWS S3
1. Log in to your AWS account.
2. Navigate to the S3 service.
3. Click 'Create Bucket'.
4. Give the bucket a unique name. Follow the bucket naming rules from AWS. The bucket will be named 'kelz-static-website-hosting-s3'. Reference: https://docs.aws.amazon.com/AmazonS3/latest/userguide/bucketnamingrules.html?icmpid=docs_amazons3_console
6. Disable Access Control Lists (ACLs). This will enable the owner of the bucket to control access to the bucket using policies.
7. Select Server-side encryption with Amazon S3 managed keys (SSE-S3) for the encryption type.
8. Click 'Create bucket'.
<img width="1400" alt="Screenshot 2024-05-21 at 2 44 16 PM" src="https://github.com/TallboyKelz/S3-website-kelz/assets/133192420/4d74461c-9797-4082-99cc-c50247a0320f">


# Configuring S3 for Static Hosting
1. Open the newly created bucket.
2. Go to the "Properties" tab.
3. Scroll down to "Static website hosting" and click "Edit".
4. Select "Enable" and specify the index document and error document (e.g., index.html, error.html).
5. Save changes
   
# Uploading website files
1. Go to the "Objects" tab in your S3 bucket.
2. Click "Upload" and add your website files (HTML, CSS, JS, images).
3. Click "Upload" to start the process.
<img width="1385" alt="Screenshot 2024-05-21 at 2 55 40 PM" src="https://github.com/TallboyKelz/S3-website-kelz/assets/133192420/f83741ab-84b3-4349-a02a-25f6b7be6d1e">

   
# Permissions
Now, we have to set a policy for the bucket to make it publicly accessible over the internet. To do this:
1. Go to the "Permissions" tab.
Click "Bucket Policy" and paste the following code for the policy.



# Accessing the Website
# Security Best Practices
# Conclusion
# References
