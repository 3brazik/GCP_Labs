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