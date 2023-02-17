# Kubernetes - Helm
## Kubernetes Helm Home Task
#### Task 1
* Deploy Nginx via helm with Ingress configuration:
* Set variables via value yaml
* Use “helm upgrade --install --atomic …” to change some parameters (Example: number of pods)

#### Task 2
* Create and deploy your own chart with the [Pacman](https://hub.docker.com/r/golucky5/pacman), [game](https://helm.sh/docs/chart_template_guide/getting_started/)

## Steps:

* Deploy Nginx via helm 
```
helm install nginx nginx
```
<img width="1237" alt="image" src="https://user-images.githubusercontent.com/117667360/219613023-4cb87f06-1956-40e3-ba67-9f811d074971.png">

* Change number of pods:
```
helm upgrade --atomic nginx nginx/ --set replicaCount=5
```
<img width="1236" alt="image" src="https://user-images.githubusercontent.com/117667360/219613346-131006f4-af89-414b-a828-ed26a99c0181.png">

* Nginx:

<img width="949" alt="image" src="https://user-images.githubusercontent.com/117667360/219619476-bb157896-5edd-46f9-a349-a5ddbe65b296.png">

* Deploy pacman
```
helm install pacman pacman/
```
<img width="1092" alt="image" src="https://user-images.githubusercontent.com/117667360/219620360-c0b8ba83-afa6-4cec-a7e8-826d517be534.png">

```
kubectl get pods | grep pacman
```
<img width="886" alt="image" src="https://user-images.githubusercontent.com/117667360/219615370-f204611f-203d-467f-9213-dfcda4145a6e.png">

* Pacman

![tg_image_2991993571](https://user-images.githubusercontent.com/117667360/219625861-72065c7b-eb10-45ac-9285-7ebf3053127c.jpeg)
