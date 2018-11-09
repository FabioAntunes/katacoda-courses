# Deploy RabbitMQ #

Provisioning RabbitMQ on Kubernetes is easily done by invoking this [stable Helm chart](https://github.com/helm/charts/tree/master/stable/rabbitmq).  

`helm install stable/rabbit-ha --name my-rabbit --namespace rabbit -f rabbit-values.yaml`{{execute}}

The RabbitMQ containers start fairly quickly so the Pod status may be already running creating, or initializing. To get a complete status of the deployment availability run this inspection

`kubectl get deployments,pods,services --namespace rabbit`{{execute}}.

As an alternative to the kubectl CLI you can also observe the deployment in the Kubernetes Dashboard by clicking on the tab above this command line or from this link: https://[[HOST_SUBDOMAIN]]-30000-[[KATACODA_HOST]].environments.katacoda.com/