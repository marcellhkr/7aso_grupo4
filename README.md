# 7aso_grupo4
Repositório git : https://github.com/marcellhkr/7aso_grupo4

# Entregas

## Entrega 1
- **Dockerfile**: O arquivo `Dockerfile` está presente dentro do diretório blog-django-py.
- Clonamos o projeto original e geramos uma imagem docker a partir dele no repositório https://hub.docker.com/repository/docker/marcellhkr/blog-django-py
- Está imagem está sendo usada no deployment

## Entrega 2
- **Ingress**: Arquivos dentro do diretórios route e service
- **Deploy de banco de dados**: Arquivo `deployment/dp-config-sample-database.yml`
- **Camada de persistência**: Arquivo `pvc/sample-database.pvc.yml`

## Entrega 3
- **Secrets**: Diretório secret
- **HPA**: Diretório HPA

## Entrega 4
Pipeline utilizando kustomization
https://kubernetes.io/docs/tasks/manage-kubernetes-objects/kustomization/

# Deploy da aplicação

Antes de iniciar o processo, é necessário criar o projeto com o nome desejado no OpenShift. Isso pode ser feito através do comando `oc new-project nome_projeto` ou através do console web do cluster.

Para criar toda a infra, é só executar o comando `oc apply -k ./<diretorio_raiz_repositorio>` (ex.: `oc apply -k ./7aso_grupo4`).
- Para logar na aplicação use usuário e senha iguais a developer.
