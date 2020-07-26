# LibreDataStore


# Connect local kubectl to remote server

You need to first copy some Kubernetes credentials from remote Kubernetes master to your Macbook.

```
scp -r vagrant@192.168.205.10:/home/vagrant/.kube .
```
Copy the Kubernetes Credentials your downloaded to your home directory as shown below.

```
cp -r .kube $HOME/
```

That's it! Kubectl should now be conencted to the remote cluster. Try checking the current kubectl context 

```
kubectl config current-context
```

