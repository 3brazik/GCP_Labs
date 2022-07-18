# Lab 3.2

Mohamed Abdelrazik 

```bash
1. Using gsutil:
```

```bash
– Create 3 buckets.
```

![Screenshot from 2022-06-26 01-18-33.png](Lab%203%202%20e8505cb50e0c4e09a7d897fdf0ef0619/Screenshot_from_2022-06-26_01-18-33.png)

![Screenshot from 2022-06-26 01-19-13.png](Lab%203%202%20e8505cb50e0c4e09a7d897fdf0ef0619/Screenshot_from_2022-06-26_01-19-13.png)

```bash
– Enable Versioning for them.
```

![Screenshot from 2022-06-26 01-18-55.png](Lab%203%202%20e8505cb50e0c4e09a7d897fdf0ef0619/Screenshot_from_2022-06-26_01-18-55.png)

```bash
– Upload a file into bucket-1 3
```

![Screenshot from 2022-06-26 01-37-55.png](Lab%203%202%20e8505cb50e0c4e09a7d897fdf0ef0619/Screenshot_from_2022-06-26_01-37-55.png)

![Screenshot from 2022-06-26 01-38-45.png](Lab%203%202%20e8505cb50e0c4e09a7d897fdf0ef0619/Screenshot_from_2022-06-26_01-38-45.png)

```bash
then copy it from bucket-1 into bucket-2 & bucket-3
```

![Screenshot from 2022-06-26 01-39-44.png](Lab%203%202%20e8505cb50e0c4e09a7d897fdf0ef0619/Screenshot_from_2022-06-26_01-39-44.png)

```bash
– Delete the file from bucket-1
```

![Untitled](Lab%203%202%20e8505cb50e0c4e09a7d897fdf0ef0619/Untitled.png)

![Screenshot from 2022-06-26 01-41-55.png](Lab%203%202%20e8505cb50e0c4e09a7d897fdf0ef0619/Screenshot_from_2022-06-26_01-41-55.png)

```bash
2. Host a static website on a standard public GCS bucket.

	
```

![Screenshot from 2022-06-26 02-12-51.png](Lab%203%202%20e8505cb50e0c4e09a7d897fdf0ef0619/Screenshot_from_2022-06-26_02-12-51.png)

![Screenshot from 2022-06-26 02-13-58.png](Lab%203%202%20e8505cb50e0c4e09a7d897fdf0ef0619/Screenshot_from_2022-06-26_02-13-58.png)

![Screenshot from 2022-06-26 02-35-59.png](Lab%203%202%20e8505cb50e0c4e09a7d897fdf0ef0619/Screenshot_from_2022-06-26_02-35-59.png)

![Screenshot from 2022-06-26 02-39-28.png](Lab%203%202%20e8505cb50e0c4e09a7d897fdf0ef0619/Screenshot_from_2022-06-26_02-39-28.png)

![Screenshot from 2022-06-26 02-37-49.png](Lab%203%202%20e8505cb50e0c4e09a7d897fdf0ef0619/Screenshot_from_2022-06-26_02-37-49.png)

```bash
3. Deploy MySQL private instance and connect to it then create a new database.
```

```bash
Create a Cloud SQL instance with a private IP address
```

![Screenshot from 2022-06-26 03-50-16.png](Lab%203%202%20e8505cb50e0c4e09a7d897fdf0ef0619/Screenshot_from_2022-06-26_03-50-16.png)

```bash
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

```bash
then create Database new_db
```

![Screenshot from 2022-06-26 04-05-16.png](Lab%203%202%20e8505cb50e0c4e09a7d897fdf0ef0619/Screenshot_from_2022-06-26_04-05-16.png)