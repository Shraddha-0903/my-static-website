# My Awesome Project

Welcome to my awesome project! Here is a link to view my static website hosted on AWS:

**Live Demo**: http://shraddhaa.click/

*Step 1: Create an S3 Bucket*
Log in to the AWS Management Console.
Navigate to S3 from the Services menu.
Click on the Create bucket button.
Choose a unique name for your bucket (e.g., my-static-website-bucket).
The bucket name must be globally unique, so pick a name that’s not already in use.
Choose a region close to your audience (e.g., US East (N. Virginia)).
Scroll down and disable block public access settings (this is required for hosting a website).
Warning: Ensure you're only allowing public access to the files that are meant to be public (website content).
Click Create bucket.

*Step 2: Upload Website Files*
Open the S3 bucket you just created.
Click on Upload.
Drag and drop your website files (HTML, CSS, JS, images) into the bucket, or choose them manually.
Make sure your index.html is included as it will be your website’s homepage.
After uploading, select all files, then click Actions > Make public to allow access to them.

*Step 3: Enable Static Website Hosting*
Go to the Properties tab of your S3 bucket.
Scroll down to the Static website hosting section and click Edit.
Select Enable.
For Index document, enter index.html (or your homepage file name).
For Error document, you can set it to error.html (optional).
Click Save changes.

*Step 4: Access Your Static Website*
In the Static website hosting section, you will see a URL for your website.
Open this URL in your browser, and you should see your static website live!

*Step 5: Set Up a Custom Domain*
To set up a custom domain for your website, follow these additional steps:
Purchase a Domain: Use a domain provider like Route 53, purchase a domain.
Create a Hosted Zone: In Route 53, create a hosted zone for your domain.
Create a Record Set: Add a record set that points your domain to the S3 website endpoint (found in the Static Website Hosting section).
Configure DNS: Update the DNS records at your domain registrar to point to the Route 53 hosted zone.

And there you have it – your very own static website hosted on AWS S3. 🚀
