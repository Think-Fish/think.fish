# [think.fish](http://www.think.fish)

### Deploying

 `gsutil cp TARGET_DEPLOY_NAME.html gs://NAME_OF_STATIC_STORAGE_BUCKET && gsutil cp TARGET_DEPLOY_NAME.html gs://www.NAME_OF_STATIC_STORAGE_BUCKET`

 `gsutil acl ch -u AllUsers:R gs://NAME_OF_STATIC_STORAGE_BUCKET &&  gsutil acl ch -u AllUsers:R gs://www.NAME_OF_STATIC_STORAGE_BUCKET `

 `gsutil defacl ch -u AllUsers:R gs://NAME_OF_STATIC_STORAGE_BUCKET &&  gsutil acl ch -u AllUsers:R gs://www.NAME_OF_STATIC_STORAGE_BUCKET `
