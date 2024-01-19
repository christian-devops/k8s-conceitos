# Instalação da aplicação Odoo via Helm

Adicionar o Repo

```bash
helm repo add bitnami https://charts.bitnami.com/bitnami
helm repo update
```

Instalar 

```bash

helm upgrade -i odoo bitnami/odoo --version 25.2.1 \
    -n treinamento \
    --values values.yaml \
    --create-namespace
```