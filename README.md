# Google Cloud Functions with Python

## This is a Udemy Cource created by David Armendáriz

To start a new Project goto the [Firebase Console](https://console.firebase.google.com/) or create from the [Google Cloud Console](https://console.cloud.google.com/)

## Quick Setup
Get started by creating a new file or uploading an existing file. We recommend every repository include a README, LICENSE, and .gitignore.

…or create a new repository on the command line
echo "# google-cloud-functions-python" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin git@github.com:vipul-garg/google-cloud-functions-python.git
git push -u origin main

…or push an existing repository from the command line
git remote add origin git@github.com:vipul-garg/google-cloud-functions-python.git
git branch -M main
git push -u origin main

## Create a python virtual environment
First install python3-venv
```
sudo apt install python3-venv
```
Then run the following command
``` 
python3 -m venv venv
```

Activate the python virtual environment
```
source venv/bin/activate
```

To install the python package requirements run the following:
```
pip install -r requirements.txt
```

## Deploying the function
First, we have to set our project ID with the following command:
```
gcloud config set project [YOUR_PROJECT_ID]
```
Then we deploy our function with this command:
```
gcloud functions deploy [FUNCTION_NAME] --runtime python37 --trigger-http
```