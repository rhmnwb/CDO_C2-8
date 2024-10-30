# Configure S3 Bucket
## Step 1: Enable website hosting
#### Reference: [https://docs.aws.amazon.com/cli/latest/reference/s3/website.html#examples](https://docs.aws.amazon.com/cli/latest/reference/s3/website.html#examples)
```
aws s3 website s3://cdo-c2.8-167029074152-bucket/ --index-document index.html --error-document error.html
```

## Screenshots
#### Website hosting enabled
<img width="1579" alt="image" src="https://github.com/user-attachments/assets/2ec1a603-999a-4ead-82cc-ea6ee1ec1f61">

#### Website accessible via HTTP
<img width="1280" alt="image" src="https://github.com/user-attachments/assets/de09cc68-7ff3-4fbf-872f-f64b9ece1c8b">
