# Computacao_em_nuvem_Aula5

códigos
**Passo 1:**
 Erick: kubectl version --client
 Retorno:
 
Client Version: v1.37.1
Kustomize Version: v5.8.1


**Passo 2:**
Erick: kubectl get nodes
Retorno:

NAME           STATUS   ROLES           AGE   VERSION
controlplane   Ready    control-plane   9d    v1.37.1
node01         Ready    <none>          9d    v1.37.1


**Passo 3:**
Erick: kubectl create deployment web-aula5 --image=nginx:alpine
Retorno:

deployment.apps/web-aula5 created


**Passo 4:**
Erick: kubectl get deployments
Retorno:

NAME        READY   UP-TO-DATE   AVAILABLE   AGE
web-aula5   1/1     1            1           14s


**Passo 5:**
Erick: kubectl get pods
Retorno:

NAME                         READY   STATUS    RESTARTS   AGE
web-aula5-779c6f9566-xbxgx   1/1     Running   0          3m43s
