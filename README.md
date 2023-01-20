# tf-deploy-nginix-kubernetes




 



<h2>Description</h2>

Building kubernetes cluster to deploy nginx resource using Terraform 
https://developer.hashicorp.com/terraform/tutorials/kubernetes/kubernetes-provider





<br />





<h2>Languages and Utilities Used</h2>



- <b>kubernetes</b> 

- <b>Terraform </b>



<h2>Environments Used </h2>



- <b></b>

- <b>Ubuntu 22.04</b>



<h2>Program walk-through:</h2>


First, I had to install kubectl following the install doc

https://kubernetes.io/docs/tasks/tools/install-kubectl-linux/#install-using-native-package-management

Once that was installed, I then installed kind to build the cluster.

https://kind.sigs.k8s.io/docs/user/quick-start

once both were installed I created the cluster and pulled the cluster info to add to terraform.tfvars.

with the variables set, I deployed the cluster using terraform and validated the deployment using kubectl



![cluster dump](https://user-images.githubusercontent.com/85902399/213818370-33c299ae-5b47-4255-916e-69f52c69969f.png)







<br/>

<br/>



With the cluster validated, I verified Nginx was deployed using the localhost ip.



<br />

<br />

![verify-nginx-loaded](https://user-images.githubusercontent.com/85902399/213818475-c3aa7a10-2214-49fd-adc3-c1d1b5f98df1.png)






