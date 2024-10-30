# Step 1: Create the bucket
aws s3api create-bucket --bucket cdo-c2.8-167029074152-bucket --region us-east-1

# Step 2: Set public access block configuration to allow public access
# Reference: https://awscli.amazonaws.com/v2/documentation/api/latest/reference/s3api/put-public-access-block.html
aws s3api put-public-access-block --bucket cdo-c2.8-167029074152-bucket --public-access-block-configuration BlockPublicAcls=false,IgnorePublicAcls=false,BlockPublicPolicy=false,RestrictPublicBuckets=false
