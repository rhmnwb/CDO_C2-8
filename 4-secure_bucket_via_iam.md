# Secure Bucket via IAM
## Step 1: Update policy
#### Reference: [https://awscli.amazonaws.com/v2/documentation/api/latest/reference/s3api/put-public-access-block.html](https://docs.aws.amazon.com/AmazonS3/latest/userguide/access-control-block-public-access.html)
```
aws s3api put-bucket-policy --bucket cdo-c2.8-167029074152-bucket --policy '{
   "Version": "2012-10-17",
   "Statement": [
      {
         "Effect": "Allow",
         "Principal": "*",
         "Action": "s3:GetObject",
         "Resource": "arn:aws:s3:::cdo-c2.8-167029074152-bucket/*"
      }
   ]
}'
```

## Screenshots
#### Policy updated
<img width="1588" alt="image" src="https://github.com/user-attachments/assets/54429e92-7145-4ec0-8c34-3ad3626534ed">
