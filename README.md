# Project-2-Sports-Person-Classifier
![](project_image.png)

# Introduction -
In this data science project I walked through the process of building a Sports Person Classifier website. I first built a model using sklearn and logistic regression using images of multiple celebrities. Second step was to create a python flask server that uses the saved model to serve http requests. Third component was the website built using html, css and javascript that allows user to upload images and it calls the python flask server to retrieve the result. During model building I covered many data science concepts such as data load and cleaning, outlier detection and removal, feature engineering, gridsearchcv for hyperparameter tunning, etc. I enjoyed creating this project and I hope you like it😊

# Tools used to create the project-
1. Python
2. Numpy and pandas for data cleaning
3. Matplotlib for data visualization
4. Sklearn for model building
5. Jupyter Notebook in Visual Studio Code as IDE
6. Python flask server for http server
7. HTML/CSS/Javascript for UI

# Deploy this app to cloud (GCP VM)-

1. Create VM instance using google cloud console and allow HTTP/HTTPS incoming traffic while setting the VM.
2. Generate SSH keys using PuTTYgen and save the private key with you and upload the key under the SSH Keys section in the settings of the VM.
3. Now connect to your instance using PuTTY windows application.
4. Become the root user to avoid permission errors with the command-
```
sudo su
```
5. Update the linux instance and install nginx using using the commands-
```
sudo apt-get update
sudo apt-get install nginx
```
6. We can check whether the nginx server is running by loading the url of the instance in the browser.
7. Now login to your instance and transfer the application folder (download this repo, extract it and rename the folder as SportsPersonClassifier, this folder is now your application folder😊) into the VM instance using WinSCP application.
8. Navigate to the location using the command-
```
cd /etc/nginx/sites-enabled
```
9. Unlink the deafult file using the command-
```
sudo unlink default
```
10. Navigate to the location using the command-
```
cd /etc/nginx/sites-available
```
11. 
