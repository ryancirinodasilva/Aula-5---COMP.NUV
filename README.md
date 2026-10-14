# Aula-5---COMP.NUV

## Atividade prática — Kubernetes
• Abrir um ambiente Kubernetes no Killercoda.
• Conhecer o cluster com kubectl.
• Criar um Deployment com Nginx.
• Observar o Pod criado.
• Escalar de 1 para 3 réplicas.
• Excluir um Pod e observar a autorrecuperação.
• Expor e testar a aplicação dentro do cluster.

### Prática — Passo 1: entrar no Killercoda
https://killercoda.com/playgrounds/course/kubernetes-playgrounds/two-node
• Faça login na conta gratuita.
• Abra o Kubernetes Playground de dois nós.
• Aguarde o terminal e o cluster ficarem disponíveis.
• O ambiente gratuito é temporário: conclua a prática dentro da aula.

### Prática — Passo 2: o cluster está funcionando?
kubectl version --client

kubectl get nodes

### Prática — Passo 3: criar nossa aplicação
kubectl create deployment web-aula5 --image=nginx:alpine

kubectl get deployments

### Prática — Passo 4: onde está o Pod?
kubectl get pods

kubectl get pods -o wide

