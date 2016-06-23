# Rotate TLS Certificate for CloudFront

Upload a new TLS certificate to CloudFront.

If a previous certificate was uploaded, change the `--server-certificate-name` to something
different and select the new name in the CloudFront distribution.

```
aws iam upload-server-certificate --server-certificate-name test.com-2016 --certificate-body file://test_com.crt --private-key file://test_com.pem --certificate-chain file://test_com.ca-bundle --path /cloudfront/
```
