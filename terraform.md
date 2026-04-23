# Linha do Tempo de Estudos — Terraform

## Fase 1 — Fundamentos (Semanas 1–2)
- [ ] O que é Infrastructure as Code (IaC) e por que usar
- [ ] Instalação do Terraform e configuração do ambiente
- [ ] Estrutura básica de um arquivo `.tf`: `provider`, `resource`, `variable`, `output`
- [ ] Providers: AWS, Azure, GCP — como configurar credenciais
- [ ] Comandos essenciais: `init`, `plan`, `apply`, `destroy`
- [ ] Entender o `terraform.tfstate` e por que ele é crítico

## Fase 2 — Conceitos Intermediários (Semanas 3–4)
- [ ] Variáveis de entrada (`variable`) e saída (`output`)
- [ ] Arquivo `terraform.tfvars` e `.auto.tfvars`
- [ ] Data sources: consultar recursos existentes sem criar
- [ ] Módulos locais: como criar e reutilizar módulos
- [ ] Módulos públicos do Terraform Registry
- [ ] `depends_on`, `count` e `for_each` para recursos dinâmicos
- [ ] Funções built-in: `join`, `split`, `lookup`, `length`, `toset`

## Fase 3 — State e Backends (Semana 5)
- [ ] Remote state: armazenar o `.tfstate` no S3 com DynamoDB para lock
- [ ] `terraform workspace`: ambientes dev, staging, prod
- [ ] Import de recursos existentes com `terraform import`
- [ ] `terraform taint` e `terraform untaint`
- [ ] Estratégias de versionamento do state

## Fase 4 — Boas Práticas e Estrutura de Projetos (Semana 6)
- [ ] Estrutura de pastas para projetos reais (monorepo vs multi-repo)
- [ ] Separação por ambiente: `environments/dev`, `environments/prod`
- [ ] Uso de `locals` para reduzir repetição
- [ ] Validação de variáveis com `validation` block
- [ ] `terraform fmt` e `terraform validate` no CI
- [ ] Ferramentas complementares: `tflint`, `checkov`, `infracost`

## Fase 5 — Terraform com AWS (Semanas 7–8)
- [ ] Provisionar VPC, subnets, security groups
- [ ] EC2: instâncias, key pairs, user data
- [ ] RDS: banco de dados gerenciado
- [ ] S3: buckets com versionamento e lifecycle
- [ ] IAM: roles, policies e usuários via Terraform
- [ ] Load Balancer (ALB) e Auto Scaling Group
- [ ] EKS cluster via Terraform (integração com Kubernetes)

## Fase 6 — Avançado (Semanas 9–10)
- [ ] Terraform Cloud e Terraform Enterprise
- [ ] Sentinel: policy as code
- [ ] `terraform graph` para visualizar dependências
- [ ] Migração de recursos entre states
- [ ] Terragrunt: wrapper para DRY em grandes projetos
- [ ] Projeto final: infraestrutura completa de uma aplicação na AWS

## Recursos Recomendados
- Documentação oficial: https://developer.hashicorp.com/terraform/docs
- Curso: HashiCorp Certified Terraform Associate
- Repositório de exemplos: terraform-aws-modules no GitHub
- Livro: "Terraform: Up & Running" — Yevgeniy Brikman
