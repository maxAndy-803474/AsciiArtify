# Create a new application in ArgoCD

![Screenshot of a Argocd.](https://github.com/maxAndy-803474/AsciiArtify/blob/main/31.png)

## Add port forwarding

```
kubectl port-forward -n demo svc/ambassador 8088:80
```

## Download random png file

```
wget -O /tmp/g.png https://www.google.com/images/branding/googlelogo/1x/googlelogo_color_272x92dp.png
```

## Upload this file to the converter

```
curl -F 'image=@/tmp/g.png' localhost:8088/img/
```
You should observe something like this

![Screenshot of a MVP.](https://github.com/maxAndy-803474/AsciiArtify/blob/main/10.png)

