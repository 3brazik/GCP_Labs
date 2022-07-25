# GCP_Labs
# Lab 1.1

```plain text
1.Explore Google Cloud Console.
Done
```

```plain text
2.Setup a billing method on your google account.
3.Create a GCP project.
4.Assign your billing account to your project.
5.Setup project budget.
6.Setup billing alerts.
	
	Hosted By Mostafa Elnaggar Brother Mohamed elNaggar
```

```plain text
7.Using cloud shell, list all projects and set default project.
```

![Screenshot from 2022-06-22 22-06-58.png](Lab%201%201%20f786275f4b5c4619ab8e921884ebd688/Screenshot_from_2022-06-22_22-06-58.png)

![Screenshot from 2022-06-22 22-22-03.png](Lab%201%201%20f786275f4b5c4619ab8e921884ebd688/Screenshot_from_2022-06-22_22-22-03.png)

```plain text
8.Install and configure gcloud SDK on your pc.
Done
```

```plain text
9.List all projects using gcloud SDK and set default project1.
```

![Screenshot from 2022-06-22 22-09-06.png](Lab%201%201%20f786275f4b5c4619ab8e921884ebd688/Screenshot_from_2022-06-22_22-09-06.png)

![Screenshot from 2022-06-22 22-24-31.png](Lab%201%201%20f786275f4b5c4619ab8e921884ebd688/Screenshot_from_2022-06-22_22-24-31.png)

# Lab 1.2

```bash
I.Create custom role named "my-custom-role-1" with the following permissions only:
– Iam.roles.get
– Iam.roles.list
```

![Screenshot from 2022-06-22 22-56-28.png](Lab%201%201%20f786275f4b5c4619ab8e921884ebd688/Screenshot_from_2022-06-22_22-56-28.png)

![Screenshot from 2022-06-22 22-54-50.png](Lab%201%201%20f786275f4b5c4619ab8e921884ebd688/Screenshot_from_2022-06-22_22-54-50.png)

```plain text
2.From Cloud console, Explore primitive and pre-defined roles and their permissions.
```

![Screenshot from 2022-06-22 22-59-16.png](Lab%201%201%20f786275f4b5c4619ab8e921884ebd688/Screenshot_from_2022-06-22_22-59-16.png)

![Screenshot from 2022-06-22 22-58-33.png](Lab%201%201%20f786275f4b5c4619ab8e921884ebd688/Screenshot_from_2022-06-22_22-58-33.png)

![Screenshot from 2022-06-22 23-02-28.png](Lab%201%201%20f786275f4b5c4619ab8e921884ebd688/Screenshot_from_2022-06-22_23-02-28.png)

```plain text
3.From Cloud console, Create a service account with id "my-first-serviceaccount".
```

![Screenshot from 2022-06-22 23-09-26.png](Lab%201%201%20f786275f4b5c4619ab8e921884ebd688/Screenshot_from_2022-06-22_23-09-26.png)

```plain text
4.From Cloud console, Assign the custom role "my-custom-role-1" to the service
account "my-first-serviceaccount"
```

![Screenshot from 2022-06-22 23-16-53.png](Lab%201%201%20f786275f4b5c4619ab8e921884ebd688/Screenshot_from_2022-06-22_23-16-53.png)

```plain text
5.Using gcloud,
I.List all roles on your project.

```

![Screenshot from 2022-06-22 23-21-20.png](Lab%201%201%20f786275f4b5c4619ab8e921884ebd688/Screenshot_from_2022-06-22_23-21-20.png)

```plain text
II.Describe the predefined role "roles/compute.viewer" and view its details & permissions
```

![Screenshot from 2022-06-22 23-27-05.png](Lab%201%201%20f786275f4b5c4619ab8e921884ebd688/Screenshot_from_2022-06-22_23-27-05.png)

```plain text
III.Describe the custom role "my-custom-role-1" and view its details & permissions.

```

![Screenshot from 2022-06-22 23-36-52.png](Lab%201%201%20f786275f4b5c4619ab8e921884ebd688/Screenshot_from_2022-06-22_23-36-52.png)

```plain text

IV.List all authenticated accounts.

```

![Screenshot from 2022-06-22 23-39-34.png](Lab%201%201%20f786275f4b5c4619ab8e921884ebd688/Screenshot_from_2022-06-22_23-39-34.png)

```plain text

V.Activate the service account "my-first-serviceaccount".

```

![Screenshot from 2022-06-22 23-44-30.png](Lab%201%201%20f786275f4b5c4619ab8e921884ebd688/Screenshot_from_2022-06-22_23-44-30.png)

```plain text

VI.List all authenticated accounts again.

```

![Screenshot from 2022-06-22 23-44-56.png](Lab%201%201%20f786275f4b5c4619ab8e921884ebd688/Screenshot_from_2022-06-22_23-44-56.png)

```plain text

VII.Using this service account, try to list all roles on your project.
```

![Screenshot from 2022-06-22 23-59-21.png](Lab%201%201%20f786275f4b5c4619ab8e921884ebd688/Screenshot_from_2022-06-22_23-59-21.png)

```plain text
VIII.Try to delete custom role "my-custom-role-1"

```

![Screenshot from 2022-06-23 00-01-03.png](Lab%201%201%20f786275f4b5c4619ab8e921884ebd688/Screenshot_from_2022-06-23_00-01-03.png)








# Lab 2




Lab 2.1

```plain text
1-From Cloud console, create a VPC named “auto-vpc” with auto-mode enabled,
How many subnets created? And how many routes created for this VPC? Can you delete any of
these routes?
```

![Screenshot from 2022-06-23 21-08-03.png](Lab%202%20bf0bb66b1ea44e079f385fc3f67bca39/Screenshot_from_2022-06-23_21-08-03.png)

![Screenshot from 2022-06-23 21-04-18.png](Lab%202%20bf0bb66b1ea44e079f385fc3f67bca39/Screenshot_from_2022-06-23_21-04-18.png)

  

```plain text
		34 subnets
```

```plain text
		35 Route
```

```plain text
Local routes cannot be deleted  
only public route can be deleted
```

```plain text
2-From Cloud console, create a VPC named “custom-vpc” with auto-mode disabled and create two
subnets. How many routes created for this VPC?
```

```plain text
3 Route
 1 for public 
	and 2 for subnets
```

![Screenshot from 2022-06-23 21-25-37.png](Lab%202%20bf0bb66b1ea44e079f385fc3f67bca39/Screenshot_from_2022-06-23_21-25-37.png)

```plain text
3-Using gcloud tool list all available VPCs and list subnets of each VPC.
```

![Screenshot from 2022-06-23 21-42-42.png](Lab%202%20bf0bb66b1ea44e079f385fc3f67bca39/Screenshot_from_2022-06-23_21-42-42.png)

```plain text
4-In two different ways, How would you block internet access from you vpc?
```

```plain text
first way we can create firewall to block internet access 
second way we can delete public route 
```

```plain text
5-Create a firewall rule to allow incoming SSH requests from internet to all instances in your vpc.
```

![Screenshot from 2022-06-23 22-51-02.png](Lab%202%20bf0bb66b1ea44e079f385fc3f67bca39/Screenshot_from_2022-06-23_22-51-02.png)

```plain text
6-Modify the previous firewall rule to allow only ssh requests coming through Google’s IAP servers.
```

![Screenshot from 2022-06-23 22-57-52.png](Lab%202%20bf0bb66b1ea44e079f385fc3f67bca39/Screenshot_from_2022-06-23_22-57-52.png)

Lab 2.2 

```plain text
1.Create a VM with public ip then:
–In two different ways, SSH into this VM.

```

![Screenshot from 2022-06-23 23-19-15.png](Lab%202%20bf0bb66b1ea44e079f385fc3f67bca39/Screenshot_from_2022-06-23_23-19-15.png)

![Screenshot from 2022-06-23 23-17-56.png](Lab%202%20bf0bb66b1ea44e079f385fc3f67bca39/Screenshot_from_2022-06-23_23-17-56.png)

![Screenshot from 2022-06-23 23-25-49.png](Lab%202%20bf0bb66b1ea44e079f385fc3f67bca39/Screenshot_from_2022-06-23_23-25-49.png)

```plain text
–Enforce SSH into this VM to be IAP protected.
```

![Screenshot from 2022-06-23 23-27-48.png](Lab%202%20bf0bb66b1ea44e079f385fc3f67bca39/Screenshot_from_2022-06-23_23-27-48.png)

```plain text
To access form cli 
gcloud compute ssh --zone=europe-west1-b instance-1 --project abdelrazek-gcp     -project --tunnel-through-iap
```

```plain text
2-Create a VM without public ip then:
	–SSH into this vm and update system packages.
```

![Untitled](Lab%202%20bf0bb66b1ea44e079f385fc3f67bca39/Untitled.png)

![Untitled](Lab%202%20bf0bb66b1ea44e079f385fc3f67bca39/Untitled%201.png)

```plain text
–Setup Nginx Web Server and test your setup.
```

![Untitled](Lab%202%20bf0bb66b1ea44e079f385fc3f67bca39/Untitled%202.png)

```plain text
–Create a custom image from this VM named “custom-img-nginx”.
```

![Untitled](Lab%202%20bf0bb66b1ea44e079f385fc3f67bca39/Untitled%203.png)

```plain text
3- Create MIG (min 3 and max 5) of a template using the custom image “custom-img-nginx”.
```

![Screenshot from 2022-06-24 20-16-58.png](Lab%202%20bf0bb66b1ea44e079f385fc3f67bca39/Screenshot_from_2022-06-24_20-16-58.png)

```plain text
4.Create a Global (or Regional) HTTP Load balancer to access your MIGs Nginx setup.
```

![Screenshot from 2022-06-24 21-13-19.png](Lab%202%20bf0bb66b1ea44e079f385fc3f67bca39/Screenshot_from_2022-06-24_21-13-19.png)

![Screenshot from 2022-06-24 21-14-17.png](Lab%202%20bf0bb66b1ea44e079f385fc3f67bca39/Screenshot_from_2022-06-24_21-14-17.png)

```plain text
Try to configure IAP at the load balancer level to protect your ingress access. Is it possible to have
IAP enabled for HTTP resources?
```

# Lab 2.2

```
1.Create a VM with public ip then:
–In two different ways, SSH into this VM.

```

![Screenshot from 2022-06-23 23-19-15.png](Lab%202%202%20c1f6e89ea3af45918a9d6f020ec5849e/Screenshot_from_2022-06-23_23-19-15.png)

![Screenshot from 2022-06-23 23-17-56.png](Lab%202%202%20c1f6e89ea3af45918a9d6f020ec5849e/Screenshot_from_2022-06-23_23-17-56.png)

![Screenshot from 2022-06-23 23-25-49.png](Lab%202%202%20c1f6e89ea3af45918a9d6f020ec5849e/Screenshot_from_2022-06-23_23-25-49.png)

```
–Enforce SSH into this VM to be IAP protected.
```

![Screenshot from 2022-06-23 23-27-48.png](Lab%202%202%20c1f6e89ea3af45918a9d6f020ec5849e/Screenshot_from_2022-06-23_23-27-48.png)

```
To access form cli 
gcloud compute ssh --zone=europe-west1-b instance-1 --project abdelrazek-gcp     -project --tunnel-through-iap
```

```
Create a VM without public ip then:
	–SSH into this vm and update system packages.
```

![Untitled](Lab%202%202%20c1f6e89ea3af45918a9d6f020ec5849e/Untitled.png)

![Untitled](Lab%202%202%20c1f6e89ea3af45918a9d6f020ec5849e/Untitled%201.png)

```
–Setup Nginx Web Server and test your setup.
```

![Untitled](Lab%202%202%20c1f6e89ea3af45918a9d6f020ec5849e/Untitled%202.png)

```
–Create a custom image from this VM named “custom-img-nginx”.
```

![Untitled](Lab%202%202%20c1f6e89ea3af45918a9d6f020ec5849e/Untitled%203.png)

```
Create MIG (min 3 and max 5) of a template using the custom image “custom-img-nginx”.
```

![Screenshot from 2022-06-24 20-16-58.png](Lab%202%202%20c1f6e89ea3af45918a9d6f020ec5849e/Screenshot_from_2022-06-24_20-16-58.png)

```
Create a Global (or Regional) HTTP Load balancer to access your MIGs Nginx setup.
```

![Screenshot from 2022-06-24 21-13-19.png](Lab%202%202%20c1f6e89ea3af45918a9d6f020ec5849e/Screenshot_from_2022-06-24_21-13-19.png)

![Untitled](Lab%202%202%20c1f6e89ea3af45918a9d6f020ec5849e/Untitled%204.png)

![Screenshot from 2022-06-24 21-14-17.png](Lab%202%202%20c1f6e89ea3af45918a9d6f020ec5849e/Screenshot_from_2022-06-24_21-14-17.png)




# lab 3

```plain text
1.Create a private GKE cluster.
```

[](https://www.notion.so/d128d3af1f0f4a37b72dc0406b4ec02a)

![Screenshot from 2022-06-24 22-23-09.png](lab%203%2006f8ebf790654947b6c6253362c9daef/Screenshot_from_2022-06-24_22-23-09.png)

```plain text
2.Deploy Nginx as a deployment using latest Nginx docker image on Docker Hub.

```

![Screenshot from 2022-06-24 22-30-13.png](lab%203%2006f8ebf790654947b6c6253362c9daef/Screenshot_from_2022-06-24_22-30-13.png)

```plain text
3.Expose your Nginx deployment using Kubernetes LoadBalancer Service.

```

![Screenshot from 2022-06-24 22-32-48.png](lab%203%2006f8ebf790654947b6c6253362c9daef/Screenshot_from_2022-06-24_22-32-48.png)

![Screenshot from 2022-06-24 22-33-11.png](lab%203%2006f8ebf790654947b6c6253362c9daef/Screenshot_from_2022-06-24_22-33-11.png)

```plain text
4.What is the type of GCP Load Balancer that is created for your LB service?

```

![Screenshot from 2022-06-24 22-37-11.png](lab%203%2006f8ebf790654947b6c6253362c9daef/Screenshot_from_2022-06-24_22-37-11.png)

```plain text
5.Use kubectl to view container logs.

```

![Screenshot from 2022-06-25 00-25-35.png](lab%203%2006f8ebf790654947b6c6253362c9daef/Screenshot_from_2022-06-25_00-25-35.png)

```plain text
6.Use cloud logging service to view container logs. [hint: search about cloud logging service for gke]
```

![Screenshot from 2022-06-25 00-35-47.png](lab%203%2006f8ebf790654947b6c6253362c9daef/Screenshot_from_2022-06-25_00-35-47.png)

```plain text
7.(Bonus) setup a HTTP load balancer for your deployment using the kubernetes ingress resource. (hint: link)
```

```plain text
8.Create an autopilot GKE cluster with public control plane.

```

![Screenshot from 2022-06-25 00-50-38.png](lab%203%2006f8ebf790654947b6c6253362c9daef/Screenshot_from_2022-06-25_00-50-38.png)

[https://www.notion.so](https://www.notion.so)

```plain text
9.Enforce the cluster’s control plane to accept only connections from your local machine.

```

![Screenshot from 2022-06-25 00-42-39.png](lab%203%2006f8ebf790654947b6c6253362c9daef/Screenshot_from_2022-06-25_00-42-39.png)

```plain text
10.Install kubectl on local machine and use it to connect to the cluster.
```

![Untitled](lab%203%2006f8ebf790654947b6c6253362c9daef/Untitled.png)

# Lab 3.2

Mohamed Abdelrazik 

```plain text
1. Using gsutil:
```

```plain text
– Create 3 buckets.
```

![Screenshot from 2022-06-26 01-18-33.png](Lab%203%202%20e8505cb50e0c4e09a7d897fdf0ef0619/Screenshot_from_2022-06-26_01-18-33.png)

![Screenshot from 2022-06-26 01-19-13.png](Lab%203%202%20e8505cb50e0c4e09a7d897fdf0ef0619/Screenshot_from_2022-06-26_01-19-13.png)

```plain text
– Enable Versioning for them.
```

![Screenshot from 2022-06-26 01-18-55.png](Lab%203%202%20e8505cb50e0c4e09a7d897fdf0ef0619/Screenshot_from_2022-06-26_01-18-55.png)

```plain text
– Upload a file into bucket-1 3
```

![Screenshot from 2022-06-26 01-37-55.png](Lab%203%202%20e8505cb50e0c4e09a7d897fdf0ef0619/Screenshot_from_2022-06-26_01-37-55.png)

![Screenshot from 2022-06-26 01-38-45.png](Lab%203%202%20e8505cb50e0c4e09a7d897fdf0ef0619/Screenshot_from_2022-06-26_01-38-45.png)

```plain text
then copy it from bucket-1 into bucket-2 & bucket-3
```

![Screenshot from 2022-06-26 01-39-44.png](Lab%203%202%20e8505cb50e0c4e09a7d897fdf0ef0619/Screenshot_from_2022-06-26_01-39-44.png)

```plain text
– Delete the file from bucket-1
```

![Untitled](Lab%203%202%20e8505cb50e0c4e09a7d897fdf0ef0619/Untitled.png)

![Screenshot from 2022-06-26 01-41-55.png](Lab%203%202%20e8505cb50e0c4e09a7d897fdf0ef0619/Screenshot_from_2022-06-26_01-41-55.png)

```plain text
2. Host a static website on a standard public GCS bucket.

	
```

![Screenshot from 2022-06-26 02-12-51.png](Lab%203%202%20e8505cb50e0c4e09a7d897fdf0ef0619/Screenshot_from_2022-06-26_02-12-51.png)

![Screenshot from 2022-06-26 02-13-58.png](Lab%203%202%20e8505cb50e0c4e09a7d897fdf0ef0619/Screenshot_from_2022-06-26_02-13-58.png)

![Screenshot from 2022-06-26 02-35-59.png](Lab%203%202%20e8505cb50e0c4e09a7d897fdf0ef0619/Screenshot_from_2022-06-26_02-35-59.png)

![Screenshot from 2022-06-26 02-39-28.png](Lab%203%202%20e8505cb50e0c4e09a7d897fdf0ef0619/Screenshot_from_2022-06-26_02-39-28.png)

![Screenshot from 2022-06-26 02-37-49.png](Lab%203%202%20e8505cb50e0c4e09a7d897fdf0ef0619/Screenshot_from_2022-06-26_02-37-49.png)

```plain text
3. Deploy MySQL private instance and connect to it then create a new database.
```

```plain text
Create a Cloud SQL instance with a private IP address
```

![Screenshot from 2022-06-26 03-50-16.png](Lab%203%202%20e8505cb50e0c4e09a7d897fdf0ef0619/Screenshot_from_2022-06-26_03-50-16.png)

```plain text
Create a Compute Engine VM to
Open two SSH connections 
We use two windows in the VM. The first window is used to install the mysql 
client and the Cloud SQL Auth proxy, get the instance connection name, and use 
this name to start the proxy. The second window is used to connect to the Cloud SQL instance through the proxy.
```

![Screenshot from 2022-06-26 03-51-54.png](Lab%203%202%20e8505cb50e0c4e09a7d897fdf0ef0619/Screenshot_from_2022-06-26_03-51-54.png)

```markup
**Steps**:

1-Install the MySQL client from the package manager and stop the mysqld server:
		sudo apt-get update
		sudo apt-get install mariadb-server-10.5
		sudo service mysqld stop
2-Install the Cloud SQL Auth proxy
	-Install wget
		sudo apt-get install wget
-Download the Cloud SQL Auth proxy:
	wget https://dl.google.com/cloudsql/cloud_sql_proxy.linux.amd64 -O cloud_sq                l_proxy
-Make the Cloud SQL Auth proxy executable:
	chmod +x cloud_sql_proxy
3-Start the Cloud SQL Auth proxy:
./cloud_sql_proxy -instances=abdelrazek-gcp-project:us-central1:instance-1=tcp:3306
```

![Untitled](Lab%203%202%20e8505cb50e0c4e09a7d897fdf0ef0619/Untitled%201.png)

```markup
from other ssh window 
connect to  sql 
	mysql -u root -p --host 127.0.0.1 --port 3306
```

![Untitled](Lab%203%202%20e8505cb50e0c4e09a7d897fdf0ef0619/Untitled%202.png)

```plain text
then create Database new_db
```

![Screenshot from 2022-06-26 04-05-16.png](Lab%203%202%20e8505cb50e0c4e09a7d897fdf0ef0619/Screenshot_from_2022-06-26_04-05-16.png)