s3-file-uploader-js-sample
=========================

Use S3 by JavaScript on Broweser.
AWS SDK for Javascript is required.

## Sample Features
- Downloads file from S3 bucket
- Uploads to S3 bucket
- Lists files in the S3 bucket

## AWS S3 CORS Settings

* Required Settings
  * AllowedMethod PUT - For #upload
  * AllowedMethod GET - For #listObjects, #getObject, #getSignedUrl
  * AllowedOrigin <site> - For all method (I think)
* ???
  * AllowedHeader

### Example
```xml
<?xml version="1.0" encoding="UTF-8"?>
<CORSConfiguration xmlns="http://s3.amazonaws.com/doc/2006-03-01/">
    <CORSRule>
        <AllowedOrigin>*</AllowedOrigin>
        <AllowedMethod>GET</AllowedMethod>
        <AllowedMethod>POST</AllowedMethod>
        <AllowedMethod>PUT</AllowedMethod>
        <MaxAgeSeconds>3000</MaxAgeSeconds>
        <AllowedHeader>*</AllowedHeader>
        <AllowedHeader>Authorization</AllowedHeader>
    </CORSRule>
</CORSConfiguration>
```

## Javascript Setttings
Copy env.js.sample to env.js, fill accessKeyId, secretAccessKey, and bucketId.

## Licence
Copyright (c) 2015 betahikaru

Released under the MIT license
