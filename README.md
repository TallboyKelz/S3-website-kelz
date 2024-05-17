<h2>Hosting A Static Website On Amazon S3</h2>

The assumption is that you already have an AWS account and have accessed it.

<h3>Disclaimer:</h3> The steps outlined below are at a high level and not very detailed.


1. Navigate to the AWS S3 resource and create a bucket.
   * The bucket should be given a name per the AWS naming rules. You can find the bucket naming rules here: https://docs.aws.amazon.com/AmazonS3/latest/userguide/bucketnamingrules.html?icmpid=docs_amazons3_console
   * Enable Access Control List (ACL) to make the bucket publicly accessible. AWS does not recommend this but we will go ahead with it for demonstration purposes.
   * Set the server-side encryption. AWS S3 SSE-S3 is recommended.
     
3. Specify the storage class. The Standard Storage class was used.
   
4. Upload the files of your website.
   
6. Enable static web hosting and specify your index document and error document.
   Tip: Place the index.html and error.html files outside the folders you uploaded in the S3 bucket.
   
8. Obtain your website's URL by navigating to the Properties tab. Under Static website hosting, you will see the Endpoint. This will be the URL of your website. In this case, the URL is: http://sample-s3-website.s3-website-us-east-1.amazonaws.com/#

