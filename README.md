# gcp-machine-learning

This is a sample of photo album application running on Google App Engine.

The uploaded photos are automatically tagged with labals in Japanese. This is done by Cloud Vision API and Cloud Translation API.

## Setup

### 1. Create a new project on Google Cloud Platform.

You can choose the region for App Engine deployment with advenced options.

### 2. Enable Vision API and Translation API from API Manager.

### 3. Open CloudShell and run the following commands.

```
$ git clone https://github.com/asashiho/gcp-machine-learning.git
$ cd gcp-machine-learning
$ pip install -r requirements.txt -t lib
$ gcloud preview datastore create-indexes index.yaml
$ gcloud app deploy
```

You can see Datastore's index creation status from Cloud Console. Please wait until the indexes are created.

That's all!
