## Steps to initialize AIRFLOW ON AWS (nov-2023 pd:aws is always changing):

1. Create EC2 instance. make sure that your instance use medium size of memory to run airflow

2. Edit inbound rules of your EC2 in order to run airflow in port 8080

3. Connect to your instance and Copy and Paste the next Commands:
   {	sudo apt update
   	sudo apt install python3-pip
	sudo apt install python3.10-venv
	python3 -m venv customer_churn_youtube_venv
	source customer_churn_youtube_venv/bin/activate 
	sudo pip install apache-airflow
	pip install apache-airflow-providers-amazon
	airflow standalone
    }

4. Connect via SSH from visual Studio to your EC2 instance.
    use config SSH file on your local machine.

## In order to run airflow:

### ** also super important in order to conect your airflow to your project on aws you need to do:

1. go to security credentials and created acces key.
(Depends on your job you need to create a connection on airflow under aws services)

2. run the command in the ec2 terminal pip install awscli

3. runt the command aws configure (after will ask for access key id, region,)



