# Threls's Public Assets README


## Install Google Cloud SDK Mac/Linux
``` bash
# 1 - Download and Install
curl https://sdk.cloud.google.com | bash 

# 2 - Login On this step, the SDK will generate a URL. Copy paste this URL into a browser, sign in, and copy/paste the code it gives you.)
gcloud auth login

# 3 - Update
gcloud components update (might need sudo)
```

## Upload to bucket
``` bash
#upload file to google cloud
gsutil -m cp -r  * gs://assets.threls.com

#Making groups of objects publicly readabl
gsutil iam ch allUsers:objectViewer gs://assets.threls.com
```
