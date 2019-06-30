# Conclusion #

OpenFaaS is an independent project created by [Alex Ellis](https://www.alexellis.io/) that is being built and shaped by a growing community of contributors. Kubernetes provides this serverless framework a resilient and scalable cluster where OpenFaaS can compliment other solutions in the same shared data center.

## Lessons Learned ##

With these steps you have learned:

- how to install OpenFaaS on Kubernetes,
- how to interact with OpenFaaS from the command line and its portal,
- how functions are deployed and removed,
- how functions are named, exposed, and invoked,
- how functions are listed, inspected and monitored,
- how functions automatically scale up and down based on load.

## References ##

- [OpenFaaS project](https://www.openfaas.com/)
- [OpenFaaS is open source](https://github.com/openfaas/faas)
- [OpenFaaS documentation](https://docs.openfaas.com/)
- [CLI tool](https://github.com/openfaas/faas-cli)
- [OpenFaaS Operator Helm chart *](https://github.com/openfaas-incubator/openfaas-operator)
- [OpenFaaS Operator Helm chart based on faas-netes Helm chart *](https://github.com/openfaas/faas-netes)
- [Helm, a package manager for Kubernetes](https://helm.sh/)
- [Helm chart for OpenFaaS](https://github.com/openfaas-incubator/openfaas-operator)
- [Video: Scaling in action with Prometheus](https://www.youtube.com/watch?v=0DbrLsUvaso)

> \* [Faas-netes chart versus OpenFaaS Operator chart](https://github.com/openfaas/faas-netes/tree/master/chart/openfaas#faas-netes-vs-openfaas-operator)
> The faas-netes controller is the most tested, stable and supported version of the OpenFaaS integration with Kubernetes. In contrast the OpenFaaS Operator (used in this scenario) is based upon the codebase and features from faas-netes, but offers a tighter integration with Kubernetes through [CustomResourceDefinitions](https://kubernetes.io/docs/concepts/extend-kubernetes/api-extension/custom-resources/) (CRD). This means you can type in `kubectl get functions` to list the CRD that make this `Kind: function` possible.

------
![No Fluff Just Stuff](/javajon/courses/kubernetes-serverless/openfaas/assets/nfjs.png "No Fluff Just Stuff")

For a deeper understanding of these topics and more join me, [Jonathan Johnson](https://nofluffjuststuff.com/conference/speaker/jonathan_johnson), for a transcendent experience on the [No Fluff Just Stuff Software Symposium Tour](https://nofluffjuststuff.com).
