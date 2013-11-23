# s3put

Upload a file to a s3 bucket. 

You can use application and deployment variables in wercker.

View this step in the [wercker directory](#TODO)

Current status on wercker:

TODO

## Options

* `key-id` (required) The Amazon Access key that will be used for authorization.
* `key-secret` (required) The Amazon Access secret that will be used for authorization.
* `bucket-url` (required) The url of the bucket to sync to, like: `s3://born2code.net`
* `source-file` (required) The local file to upload to s3.
* `dest-file` (required) The name of the file to upload to.

## Example

    - s3put:
        key-id:     $KEY
        key-secret: $SECRET
        bucket-url: $BUCKET
        source-file: myproject-0.1.0.tar.gz
        dest-file:   myproject-latest.tar.gz