# fiap-aso6-g27

Repositório para criação de infra no OpenShift

# Entregas

## Etapa 1

- **Dockerfile**: O arquivo `Dockerfile` presente na raíz

## Etapa 2

- **Ingress**: Os arquivos `route/blog-ingress.route.yml` e `service/blog.service.yml` (além das dependências dos deployments e configs)
- **Deploy de banco de dados**: O arquivo `deployment-config/sample-database.deploymentconfig.yml`
- **Camada de persistência**: O arquivo `pvc/sample-database.pvc.yml`

## Etapa 3

- **Secrets**: Os arquivos `blog.secret.yml` e `sample-database.secret.yml` dentro do diretório `secret`
- **HPA**: O arquivo `blog.hpa.yml` dentro do diretório `hpa`

## Etapa 4

O arquivo `kustomization.yml` é o arquivo principal para provisionar a infra completa em uma conta que possua o projeto `fiap` previamente criado.

# Criando o ambiente do zero no Openshift

Antes de iniciar o processo, é necessário criar o projeto `fiap` no OpenShift. Isso pode ser feito através do comando `oc new-project` ou através do console web do cluster.

Após isso ser feito, basta selecionar o projeto `fiap` no Openshift client com o comando `oc project fiap`.

Para criar toda a infra, é só executar o comando `oc apply -k ./<caminho-repositorio>` (ex.: `oc apply -k ./fiap-aso6-g27`).
Esse comando precisa indicar o diretório onde o arquivo `kustomization.yml` está. 

Após realizado o comando, os recursos no cluster serão provisionados automaticamente. 

## Projeto do grupo 27 GIT

https://github.com/LucasLeite0212/fiap-aso6-g27
