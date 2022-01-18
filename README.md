 fiap-aso6-g27

Entrega Solution Sprint - Fase 4

# Entregas

## Etapa 1

- **Dockerfile**: O arquivo `Dockerfile` presente na raíz

## Etapa 2

- **Ingress**: Os arquivos `route/blog-ingress.route.yml` e `service/blog.service.yml` com suas dependências de deployments e configs
- **Deploy de banco de dados**: Arquivo `deployment-config/sample-database.deploymentconfig.yml`
- **Camada de persistência**: Arquivo `pvc/sample-database.pvc.yml`

## Etapa 3

- **Secrets**:Arquivos `blog.secret.yml` e `sample-database.secret.yml` dentro do diretório `secret`
- **HPA**: O arquivo `blog.hpa.yml` dentro do diretório `hpa`

## Etapa 4

Com a conta fiap previamente criada será possível provisionar a infra completa com o arquivo `kustomization.yml`.
