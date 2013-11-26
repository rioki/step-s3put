# s3put

[Wercker] step to upload a file to [Amazon S3]. 

You can use application and deployment variables in wercker.

View this step in the [wercker directory][wd]

Current status on wercker:

[![wercker status](https://app.wercker.com/status/576477b5c41a585aa848dbcc6bfe58f9/m "wercker status")](https://app.wercker.com/project/bykey/576477b5c41a585aa848dbcc6bfe58f9)

## Options

* `key-id` (required) The Amazon Access key that will be used for authorization.
* `key-secret` (required) The Amazon Access secret that will be used for authorization.
* `url` (required) The S3 URL denoting the file's destination.
* `file` (required) The name of the file to upload to.

## Example

    - s3put:
        key-id:     $KEY
        key-secret: $SECRET
        file:       myproject-0.1.0.tar.gz
        url:        s3://mybucket/myproject-latest.tar.gz
        
[Wercker]: http://wercker.com
[Amazon S3]: http://aws.amazon.com/s3
[wd]: https://app.wercker.com/#applications/5290b7c2f0bb53d73e00a03c/tab/details
