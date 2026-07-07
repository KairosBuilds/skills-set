# Examples
Chain Example:
1. Secrets scanner finds AWS key in env file → Critical
2. Cloud security reviewer finds S3 bucket with public access → High
3. Combined: AWS key + public S3 = data exfiltration path → Critical
