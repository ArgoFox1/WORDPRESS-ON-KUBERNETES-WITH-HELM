# WORDPRESS-ON-KUBERNETES-WITH-HELM
![photo](https://github.com/ArgoFox1/DeployingAppInKubernetesUsingHelm/assets/105239243/4faf21c3-6404-448a-bf3f-dcb424a65587) 
![WordPress_blue_logo svg](https://github.com/ArgoFox1/DeployingAppInKubernetesUsingHelm/assets/105239243/a7fc87de-6bc4-4e57-813c-548ff77f3d2e)


# GUIDE FOR SET UP
1-**Start minikube**
>minikube start

2-**Search for the wordpress named bitnami/wordpress on website https://artifacthub.io/**

3-**Add bitnami to your repo**
>helm repo add bitnami https://charts.bitnami.com/bitnami

4-**Update your repo before installation**
>helm repo update

6-**Then create your chart**
>helm create my-chart

5-**Install bitnami wordpress**
>helm install my-wordpress bitnami/wordpress

6-**Check status of the wordpress**
>helm history wordpress

7-**You can also change your service type like that**
>helm upgrade my-new-wordpress --set service.type=ClusterIP bitnami/wordpress(I change service type to clusterIP cuz i just want to deploy project on localhost)

8-**Access the service**
>minikube service my-new-wordpress
![Screenshot from 2024-07-02 08-51-54](https://github.com/ArgoFox1/DeployingAppInKubernetesUsingHelm/assets/105239243/3a9cd3df-00e1-4a53-bc29-10eb3af8d723)
