### Praciting Kubernetes deployments

tutorial: https://kubernetes.io/docs/tutorials/stateless-application/guestbook/
guestbook-php: https://github.com/kubernetes/kubernetes/tree/release-1.10/examples/guestbook

https://medium.com/google-cloud/kubernetes-nodeport-vs-loadbalancer-vs-ingress-when-should-i-use-what-922f010849e0
https://kubernetes.io/docs/concepts/services-networking/ingress/

set-up ingress service instead of standard load balancer

useful images:
 - for performing nslookup/ping
   - `kubectl run -it --rm --restart=Never alpine --image=alpine sh`
