# Task-1-Create-a-Cloud-Storage-Bucket-and-Upload-Files


 
1. Create the S3 Bucket
 Log In: Sign in to the AWS Management Console.

 Navigate to S3: Use the search bar to find and select S3 (Simple Storage Service).

 Start Creation: Click the "Create bucket" button.
 
 Name and Region:
  
 Bucket name: Enter a globally unique name (e.g., my-unique-test-bucket-2025).
 
 AWS Region: Select your desired region (e.g., US East (N. Virginia) us-east-1).

 Block Public Access (Crucial Step):
 
 For a simple learning exercise where you want the URL to work in a browser (Step 8 of the original task), you must uncheck the box that says "Block all public access" and acknowledge the warning. Note: In a real-world scenario, you should almost always leave this checked and use signed URLs or CloudFront.
 
 Create: Leave all other settings as default and click "Create bucket".

3. Upload a File (Object)
 
 Open the Bucket: Click on the name of the bucket you just created in the S3 console list.
 
 Start Upload: Click the "Upload" button.

 Add Files: Click "Add files" or drag and drop a sample file (e.g., a .txt or .jpg file) from your computer.
 
 Set Object Permissions (Required for Public Test):
 
 In the upload flow, navigate to the "Properties" or "Permissions" step.
   
 If using ACLs, grant Read access to "Everyone (Public access)" for the object itself (this is only possible if you disabled "Block all public access" in Step 1).
 
 Finalize: Click "Upload" at the bottom of the page.

4. Verify and Test (Deliverable Outcome)

Verify Upload: Once the upload is complete, you'll see the file listed in the Objects tab of your bucket. This confirms the successful upload.

Get Public URL: Click on the name of the uploaded file/object.

Test: Copy the Object URL from the details page and paste it into a new browser tab.

Success: If you correctly configured the permissions, the file will display or download.

Failure: If you see an "Access Denied" error, the object is private, which is the default secure behavior for S3.

