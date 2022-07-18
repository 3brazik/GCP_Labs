# Lab 2

Lab 2.1

```bash
1-From Cloud console, create a VPC named “auto-vpc” with auto-mode enabled,
How many subnets created? And how many routes created for this VPC? Can you delete any of
these routes?
```

![Screenshot from 2022-06-23 21-08-03.png](Lab%202%20bf0bb66b1ea44e079f385fc3f67bca39/Screenshot_from_2022-06-23_21-08-03.png)

![Screenshot from 2022-06-23 21-04-18.png](Lab%202%20bf0bb66b1ea44e079f385fc3f67bca39/Screenshot_from_2022-06-23_21-04-18.png)

  

```bash
		34 subnets
```

```bash
		35 Route
```

```bash
Local routes cannot be deleted  
only public route can be deleted
```

```bash
2-From Cloud console, create a VPC named “custom-vpc” with auto-mode disabled and create two
subnets. How many routes created for this VPC?
```

```bash
3 Route
 1 for public 
	and 2 for subnets
```

![Screenshot from 2022-06-23 21-25-37.png](Lab%202%20bf0bb66b1ea44e079f385fc3f67bca39/Screenshot_from_2022-06-23_21-25-37.png)

```bash
3-Using gcloud tool list all available VPCs and list subnets of each VPC.
```

![Screenshot from 2022-06-23 21-42-42.png](Lab%202%20bf0bb66b1ea44e079f385fc3f67bca39/Screenshot_from_2022-06-23_21-42-42.png)

```bash
4-In two different ways, How would you block internet access from you vpc?
```

```bash
first way we can create firewall to block internet access 
second way we can delete public route 
```

```bash
5-Create a firewall rule to allow incoming SSH requests from internet to all instances in your vpc.
```

![Screenshot from 2022-06-23 22-51-02.png](Lab%202%20bf0bb66b1ea44e079f385fc3f67bca39/Screenshot_from_2022-06-23_22-51-02.png)

```bash
6-Modify the previous firewall rule to allow only ssh requests coming through Google’s IAP servers.
```

![Screenshot from 2022-06-23 22-57-52.png](Lab%202%20bf0bb66b1ea44e079f385fc3f67bca39/Screenshot_from_2022-06-23_22-57-52.png)

Lab 2.2 

```bash
1.Create a VM with public ip then:
–In two different ways, SSH into this VM.

```

![Screenshot from 2022-06-23 23-19-15.png](Lab%202%20bf0bb66b1ea44e079f385fc3f67bca39/Screenshot_from_2022-06-23_23-19-15.png)

![Screenshot from 2022-06-23 23-17-56.png](Lab%202%20bf0bb66b1ea44e079f385fc3f67bca39/Screenshot_from_2022-06-23_23-17-56.png)

![Screenshot from 2022-06-23 23-25-49.png](Lab%202%20bf0bb66b1ea44e079f385fc3f67bca39/Screenshot_from_2022-06-23_23-25-49.png)

```bash
–Enforce SSH into this VM to be IAP protected.
```

![Screenshot from 2022-06-23 23-27-48.png](Lab%202%20bf0bb66b1ea44e079f385fc3f67bca39/Screenshot_from_2022-06-23_23-27-48.png)

```bash
To access form cli 
gcloud compute ssh --zone=europe-west1-b instance-1 --project abdelrazek-gcp     -project --tunnel-through-iap
```

```bash
2-Create a VM without public ip then:
	–SSH into this vm and update system packages.
```

![Untitled](Lab%202%20bf0bb66b1ea44e079f385fc3f67bca39/Untitled.png)

![Untitled](Lab%202%20bf0bb66b1ea44e079f385fc3f67bca39/Untitled%201.png)

```bash
–Setup Nginx Web Server and test your setup.
```

![Untitled](Lab%202%20bf0bb66b1ea44e079f385fc3f67bca39/Untitled%202.png)

```bash
–Create a custom image from this VM named “custom-img-nginx”.
```

![Untitled](Lab%202%20bf0bb66b1ea44e079f385fc3f67bca39/Untitled%203.png)

```bash
3- Create MIG (min 3 and max 5) of a template using the custom image “custom-img-nginx”.
```

![Screenshot from 2022-06-24 20-16-58.png](Lab%202%20bf0bb66b1ea44e079f385fc3f67bca39/Screenshot_from_2022-06-24_20-16-58.png)

```bash
4.Create a Global (or Regional) HTTP Load balancer to access your MIGs Nginx setup.
```

![Screenshot from 2022-06-24 21-13-19.png](Lab%202%20bf0bb66b1ea44e079f385fc3f67bca39/Screenshot_from_2022-06-24_21-13-19.png)

![Screenshot from 2022-06-24 21-14-17.png](Lab%202%20bf0bb66b1ea44e079f385fc3f67bca39/Screenshot_from_2022-06-24_21-14-17.png)

```bash
Try to configure IAP at the load balancer level to protect your ingress access. Is it possible to have
IAP enabled for HTTP resources?
```