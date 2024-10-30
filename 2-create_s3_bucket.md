# Create a public S3 bucket
## Step 1: Create the bucket
```
aws s3api create-bucket --bucket cdo-c2.8-167029074152-bucket --region us-east-1
```

## Step 2: Set public-access-block-configuration to allow public access
#### Reference: [https://awscli.amazonaws.com/v2/documentation/api/latest/reference/s3api/put-public-access-block.html](https://awscli.amazonaws.com/v2/documentation/api/latest/reference/s3api/put-public-access-block.html)
```
aws s3api put-public-access-block --bucket cdo-c2.8-167029074152-bucket --public-access-block-configuration BlockPublicAcls=false,IgnorePublicAcls=false,BlockPublicPolicy=false,RestrictPublicBuckets=false
```

## Screenshots
#### Bucket created
<img width="1591" alt="image" src="https://github.com/user-attachments/assets/0223467e-0ba0-4ff5-87bc-1b9d9b104879">

#### Bucket made public
<img width="1613" alt="image" src="https://github.com/user-attachments/assets/79dd30f0-0e00-4f93-b121-a90c5d76877e">
