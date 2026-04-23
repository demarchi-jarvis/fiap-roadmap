# Linha do Tempo de Estudos — AWS

## Fase 1 — Fundamentos e Conta (Semana 1)
- [ ] Modelo de responsabilidade compartilhada AWS
- [ ] Regiões, Availability Zones e Edge Locations
- [ ] Console AWS, CLI (`aws configure`) e CloudShell
- [ ] IAM: usuários, grupos, roles e policies (JSON)
- [ ] Princípio do menor privilégio: como aplicar na prática
- [ ] AWS Organizations e multi-account strategy
- [ ] Free Tier: o que é gratuito e como evitar cobranças inesperadas
- [ ] AWS Pricing Calculator e Cost Explorer
- [ ] Billing Alerts com CloudWatch e AWS Budgets

## Fase 2 — Computação (Semanas 2–3)
- [ ] **EC2**: tipos de instância, AMIs, key pairs, Security Groups
- [ ] User Data: scripts de inicialização de instâncias
- [ ] EC2 pricing: On-Demand, Reserved, Spot, Savings Plans
- [ ] **Auto Scaling Group**: políticas de escalabilidade (Target Tracking, Step, Scheduled)
- [ ] **Load Balancers**: ALB (HTTP), NLB (TCP), GWLB (appliances)
- [ ] Target Groups e health checks
- [ ] **Lambda**: funções serverless, triggers, layers, concorrência
- [ ] **ECS**: task definitions, services, Fargate vs EC2 launch type
- [ ] **EKS**: Kubernetes gerenciado na AWS (ver kubernetes.md)
- [ ] **Elastic Beanstalk**: deploy simplificado de aplicações

## Fase 3 — Armazenamento (Semana 4)
- [ ] **S3**: buckets, objetos, classes de armazenamento (Standard, IA, Glacier)
- [ ] S3 Lifecycle policies, versionamento e replicação
- [ ] S3 presigned URLs e Block Public Access
- [ ] **EBS**: volumes SSD (gp3) e HDD, snapshots, criptografia
- [ ] **EFS**: sistema de arquivos compartilhado NFS para múltiplas instâncias
- [ ] **FSx**: para Windows (SMB) e para Lustre (HPC)
- [ ] **Storage Gateway**: bridge entre on-premises e AWS
- [ ] **DataSync**: migração e sincronização de dados

## Fase 4 — Banco de Dados (Semana 5)
- [ ] **RDS**: MySQL, PostgreSQL, MariaDB — Multi-AZ e Read Replicas
- [ ] **Aurora**: MySQL/PostgreSQL compatível, até 5x mais rápido
- [ ] Aurora Serverless v2: escala automática para workloads variáveis
- [ ] **DynamoDB**: NoSQL chave-valor, tabelas, índices (GSI, LSI)
- [ ] DynamoDB Streams e TTL
- [ ] **ElastiCache**: Redis e Memcached gerenciados
- [ ] **Redshift**: data warehouse para analytics
- [ ] **DocumentDB**: MongoDB-compatible
- [ ] **RDS Proxy**: pool de conexões para Lambda e containers

## Fase 5 — Redes e Entrega de Conteúdo (Semanas 6–7)
- [ ] **VPC**: subnets públicas e privadas, route tables, internet gateway
- [ ] **NAT Gateway**: saída de internet para subnets privadas
- [ ] **Security Groups** vs **NACLs**: stateful vs stateless
- [ ] **VPC Peering** e **Transit Gateway**: conectar múltiplas VPCs
- [ ] **VPN** e **Direct Connect**: conectar on-premises à AWS
- [ ] **Route 53**: DNS gerenciado, routing policies (weighted, latency, failover)
- [ ] **CloudFront**: CDN global, caching, OAC para S3
- [ ] **API Gateway**: REST e HTTP APIs, throttling, authorizers
- [ ] **WAF e Shield**: proteção contra DDoS e ataques web

## Fase 6 — Mensageria e Eventos (Semana 8)
- [ ] **SQS**: filas padrão e FIFO, dead-letter queue, visibility timeout
- [ ] **SNS**: pub/sub, tópicos, fanout pattern (SNS → múltiplas SQS)
- [ ] **EventBridge**: barramento de eventos, rules, targets, event patterns
- [ ] **Kinesis Data Streams**: streaming de dados em tempo real
- [ ] **Kinesis Firehose**: entrega de streams para S3, Redshift, OpenSearch
- [ ] **MSK**: Apache Kafka gerenciado
- [ ] **SES**: envio de e-mails transacionais e marketing

## Fase 7 — DevOps e Automação AWS (Semana 9)
- [ ] **CloudFormation**: IaC nativo AWS, stacks, changesets, nested stacks
- [ ] **CDK** (Cloud Development Kit): IaC com TypeScript/Python
- [ ] **CodeCommit**: repositório Git gerenciado
- [ ] **CodeBuild**: build e testes no CI
- [ ] **CodeDeploy**: deploy em EC2, ECS e Lambda (blue/green, canary)
- [ ] **CodePipeline**: orquestrar todo o fluxo CI/CD
- [ ] **Systems Manager (SSM)**: Parameter Store, Secrets, Session Manager, Patch Manager
- [ ] **CloudWatch**: métricas, logs, dashboards, alarms, Logs Insights

## Fase 8 — Segurança e Compliance (Semana 10)
- [ ] **KMS**: gerenciamento de chaves de criptografia
- [ ] **Secrets Manager**: rotação automática de secrets
- [ ] **GuardDuty**: detecção de ameaças com ML
- [ ] **Security Hub**: visão unificada de postura de segurança
- [ ] **Inspector**: scan de vulnerabilidades em EC2 e ECR
- [ ] **CloudTrail**: auditoria de todas as chamadas de API
- [ ] **Config**: monitorar conformidade de configurações
- [ ] **Macie**: detectar dados sensíveis no S3 (PII, PCI)

## Fase 9 — Arquitetura e Certificação (Semanas 11–12)
- [ ] Well-Architected Framework: 6 pilares
- [ ] Padrões de arquitetura: microserviços, serverless, event-driven
- [ ] Alta disponibilidade: Multi-AZ vs Multi-Region
- [ ] Disaster Recovery: RTO e RPO, Pilot Light, Warm Standby, Active-Active
- [ ] FinOps na AWS: Compute Optimizer, Trusted Advisor
- [ ] Simulados: AWS Skill Builder, Whizlabs, Tutorials Dojo
- [ ] Projeto final: arquitetura completa de uma aplicação production-ready na AWS

## Ordem de Certificações Sugerida
1. AWS Cloud Practitioner (CLF-C02) — base conceitual
2. AWS Solutions Architect Associate (SAA-C03) — mais valorizada
3. AWS Developer Associate (DVA-C02) — foco em código e CI/CD
4. AWS DevOps Engineer Professional (DOP-C02) — topo da trilha DevOps

## Recursos Recomendados
- AWS Skill Builder: https://skillbuilder.aws (gratuito)
- Documentação: https://docs.aws.amazon.com
- Simulados: Tutorials Dojo (Adrian Cantrill)
- Curso: Stephane Maarek no Udemy (mais completo em PT)
- Hands-on: AWS Free Tier + Cloud Quest (gamificado)
