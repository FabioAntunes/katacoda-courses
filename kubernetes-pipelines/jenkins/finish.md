# Conclusion #

You now understand fundamentally how Jenkins can run on Kubernetes. Jenkins runs the pipelines while it leverages Kubernetes to schedule the agents and to keep the engine running. Hopefully, you also understand how Kubernetes is a new type of data center _operating system_ that can run your applications - across multiple nodes on your local laptop, a rack of servers, or any cloud target.

## Technology stack ##

This demonstration was performed with these tools. Newer versions may exist.

- Kubernetes
- Kubectl
- Helm
- Prometheus Operator
- Kube-Prometheus (Alertmanager + Grafana)
- Python
- See jenkins-value.yaml file for Jenkins version and its plugins

## References ##

- [Jenkins](https://jenkins.io/)
- [Managing Resources](https://kubernetes.io/docs/concepts/cluster-administration/manage-deployment/)
- [Kubectl Cheat Sheet](https://kubernetes.io/docs/reference/kubectl/cheatsheet/)
- [Helm, a package manager for Kubernetes](https://helm.sh/)
- [Canary deployments](
https://whatis.techtarget.com/definition/canary-canary-testing)
- [Jenkins stable Helm chart](https://github.com/kubernetes/charts/tree/master/stable/jenkins)
- [Kubernetes plugin for Jenkins](https://github.com/jenkinsci/kubernetes-plugin)
- [Jenkins agent with Docker and Kubectl](https://github.com/radu-matei/jenkins-slave-docker)

## Acknowledgments ##

- A special thanks to the inspiration for this tutorial from [Chris Ricci](https://github.com/cricci82) at CoreOS (now RedHat).
- This demonstration is based on Chris Ricci and Duffie Cooley, []*Continuous Deployment and Monitoring with Tectonic, Prometheus, and Jenkins*](https://www.brighttalk.com/webcast/14601/267207/continuous-deployment-and-monitoring-with-tectonic-prometheus-and-jenkins) presentation found here on BrightTALK. Starts at the 24:15 mark.

## Etcetera ##

- Instructional video: [Lachlan Evenson's](https://github.com/lachie83/croc-hunter) demonstration [Zero to Kubernetes CI/CD in 5 minutes with Jenkins and Helm](https://youtu.be/eMOzF_xAm7w)
- Instructional video: [Continuously delivering apps to Kubernetes using Helm - Adnan Abdulhussein (Bitnami)](https://youtu.be/CmPK93hg5w8)
- [Jenkins Slave with Docker client and kubectl CLI](https://github.com/radu-matei/jenkins-slave-docker)

------
![No Fluff Just Stuff](/javajon/courses/kubernetes-pipelines/jenkins/assets/nfjs.png "No Fluff Just Stuff")

For a deeper understanding of these topics and more join me, [Jonathan Johnson](https://nofluffjuststuff.com/conference/speaker/jonathan_johnson), for a transcendent experience on the [No Fluff Just Stuff Software Symposium Tour](https://nofluffjuststuff.com).
