# ROTTEN-POTATOES
É uma simples aplicação para comentarios de filmes que foi desenvolvida para fins de teste da aula 2 a partir do treinamento INICIATIVA KUBERNETES Por FABRICIO VERONEZ .

## Como rodar o projeto?

* Pré condiçaõ Git, Docker, K3d, Kubectl instalados
* Clone esse repositório.
* Rode o ambiente com os comandos.

##-NO TERMINAL
```
git clone https://github.com/vladetec/rotten-potatoes.git
cd rotten-potatoes
cd k8s
k3d cluster create mycluster --servers 1 --agents 3 -p "8080:30000@loadbalancer"
kubectl apply -f deployment.yaml

```
## Links

[rotten-potatoes](http://localhost:8080/)

[Comandos-K3d](https://k3d.io/v5.2.2/usage/commands/)

[Comandos-Kubectl](https://kubernetes.io/docs/reference/generated/kubectl/kubectl-commands)

## Configuração

MONGODB_DB => Nome do database

MONGODB_HOST => Host do MongoDB

MONGODB_PORT => Posta de acesso ao MongoDB

MONGODB_USERNAME => Usuário do MongoDB

MONGODB_PASSWORD => Senha do MongoDB
