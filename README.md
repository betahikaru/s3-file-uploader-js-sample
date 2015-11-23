s3-file-uploder-js-sample
=========================

## AWS S3 CORS Settings

* Required Settings
  * AllowedMethod PUT - For #upload
  * AllowedMethod GET - For #listObjects, #getObject, #getSignedUrl
  * AllowedOrigin <site> - For all method (I think)
* I don't know
  * AllowedHeader

Example Setting
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

