# Examples

## Public S3 Bucket
```hcl
resource "aws_s3_bucket" "data" {
  bucket = "company-data"
  acl    = "public-read"  # Misconfiguration
}
```
