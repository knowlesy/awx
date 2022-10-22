# Getting to grips with AWX 
## AWX Testing

Study Material - I followed the links below and was able to replicate this within hyper v the YT link is faily straight forward

K8s / Kubernetes 

-[LondonIAC / Dennis McCarthy / Automation Engineer YT Guide](https://www.youtube.com/watch?v=AYfqkTbCDAw)

-[LondonIAC / Dennis McCarthy / Automation Engineer Docs](https://gist.github.com/dmccuk/93db22e9b30d1963b8fca0de96)



## Starting every session 

You can use the following code in each session to start the single node cluster and containers 



    minikube start --addons=ingress --cpus=2 --install-addons=true --kubernetes-version=stable --memory=6g

    minikube tunnel (in a seperate session)

    kubectl port-forward svc/awx-demo-service --address 0.0.0.0 30886:80
