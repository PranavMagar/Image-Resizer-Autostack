This project resizes any image uploaded to an S3 bucket.  
AutoStack will build the Docker image, push to ECR, and deploy the Lambda automatically.

## Services Used
- AWS Lambda (Container Image)
- Amazon S3
- IAM
- CloudWatch Logs

## Flow
1. Upload an image to S3.
2. Lambda (from Docker image) resizes the image to 300x300.
3. Resized image is saved to `resized/` folder inside the same bucket.

