# Linha do Tempo de Estudos — Kubernetes

## Fase 1 — Fundamentos (Semanas 1–2)
- [ ] O que é orquestração de containers e por que Kubernetes
- [ ] Arquitetura do cluster: Control Plane vs Worker Nodes
- [ ] Componentes: `kube-apiserver`, `etcd`, `scheduler`, `controller-manager`, `kubelet`, `kube-proxy`
- [ ] Instalação local: `minikube` ou `kind` (Kubernetes in Docker)
- [ ] `kubectl` — configuração, contextos e comandos básicos
- [ ] Conceito de Pod: menor unidade deployável

## Fase 2 — Objetos Essenciais (Semanas 3–4)
- [ ] **Pod**: criação, inspeção, logs e exec
- [ ] **Deployment**: réplicas, rolling update, rollback
- [ ] **ReplicaSet**: como o Deployment gerencia réplicas
- [ ] **Service**: ClusterIP, NodePort, LoadBalancer e ExternalName
- [ ] **Namespace**: isolamento lógico de recursos
- [ ] **ConfigMap** e **Secret**: configurações e dados sensíveis
- [ ] **PersistentVolume** e **PersistentVolumeClaim**: armazenamento

## Fase 3 — Redes e Exposição (Semana 5)
- [ ] Como funciona o networking interno do cluster (CNI)
- [ ] **Ingress**: roteamento HTTP/HTTPS externo com regras de host/path
- [ ] Ingress Controllers: NGINX, Traefik
- [ ] **NetworkPolicy**: controle de tráfego entre pods
- [ ] DNS interno do cluster: `<service>.<namespace>.svc.cluster.local`
- [ ] **Headless Services** para StatefulSets

## Fase 4 — Workloads Especiais (Semana 6)
- [ ] **StatefulSet**: aplicações com estado (bancos de dados)
- [ ] **DaemonSet**: um pod por node (logs, monitoramento)
- [ ] **Job** e **CronJob**: tarefas pontuais e agendadas
- [ ] **HorizontalPodAutoscaler (HPA)**: escala automática por CPU/memória
- [ ] **VerticalPodAutoscaler (VPA)**: ajuste automático de recursos
- [ ] **PodDisruptionBudget**: garantir disponibilidade durante updates

## Fase 5 — Segurança e Governança (Semanas 7–8)
- [ ] **RBAC**: Roles, ClusterRoles, RoleBindings
- [ ] **ServiceAccount**: identidade de pods para acessar a API
- [ ] **Secrets** com criptografia em repouso
- [ ] **LimitRange** e **ResourceQuota** por namespace
- [ ] **Pod Security Standards** (PSS): Restricted, Baseline, Privileged
- [ ] Scanning de imagens: Trivy, Snyk
- [ ] **OPA Gatekeeper**: policy as code para o cluster

## Fase 6 — Kubernetes na AWS — EKS (Semanas 9–10)
- [ ] Criar cluster EKS via `eksctl` e via Terraform
- [ ] Node Groups: managed vs self-managed vs Fargate
- [ ] Integração com IAM: IRSA (IAM Roles for Service Accounts)
- [ ] AWS Load Balancer Controller
- [ ] EBS CSI Driver e EFS CSI Driver para volumes
- [ ] Cluster Autoscaler e Karpenter
- [ ] Monitoramento com CloudWatch Container Insights

## Fase 7 — Observabilidade e Produção (Semanas 11–12)
- [ ] **Prometheus** + **Grafana**: métricas do cluster e aplicações
- [ ] **Loki**: agregação de logs
- [ ] **Jaeger** ou **Tempo**: tracing distribuído
- [ ] **Helm**: gerenciamento de pacotes Kubernetes
- [ ] **Kustomize**: customização de manifests por ambiente
- [ ] Projeto final: deploy de aplicação completa com HA, autoscaling e monitoramento

## Recursos Recomendados
- Documentação oficial: https://kubernetes.io/docs
- Curso: Certified Kubernetes Administrator (CKA) — Linux Foundation
- Ferramenta interativa: killer.sh (simulado CKA)
- Livro: "Kubernetes in Action" — Marko Lukša
