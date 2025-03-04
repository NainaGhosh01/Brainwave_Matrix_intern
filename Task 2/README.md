
# Static Website Hosting on Google Cloud Storage

## Project Overview
This project demonstrates how to host a static website on Google Cloud Platform (GCP) using Cloud Storage. The website consists of HTML, CSS, and images, and is accessible via a public URL.

## Technologies Used
- Google Cloud Platform (GCP)
- Cloud Storage
- HTML, CSS

## Step 1: Create a Google Cloud Storage Bucket
- Log in to the Google Cloud Console.
- Navigate to Cloud Storage under the "Storage" section.
- Click Create Bucket and configure as follows:
     - Name: my-delishus-website (must be globally unique).
    - Region: Select any (e.g., us-central1).
    - Storage Class: Standard.
    -  Access Control: Set to Uniform.
- Click Create and wait for the bucket to be created.

## Step 2: Upload Website Files
- Open the Cloud Storage bucket (my-delishus-website).
- Click Upload Folder and select your HTML folder.
- This folder should contain:
    - mainscreen.html (homepage).
    - CSS, images, and other assets.
- Wait for the files to upload successfully.

## Step 3: Make Files Public
- Open Cloud Storage → Select your bucket (my-delishus-website).
- Click on the HTML folder → Click on mainscreen.html.
- Go to the Permissions tab and click + Add.
- Enter allUsers in the New Principals field.
- Under Role, select Storage Object Viewer.
- Click Save.
- Repeat for other files (CSS, images, etc).

## Step 4: Get Public URL and Test
- Open Cloud Storage → Navigate to mainscreen.html.
- Copy the Public URL (e.g., https://storage.googleapis.com/my-delishus-website/HTML/mainscreen.html).
- Open the URL in a browser → Your website should be live! 🚀


