# Linha do Tempo de Estudos — CI/CD

## Fase 1 — Conceitos Fundamentais (Semana 1)
- [ ] O que é CI (Continuous Integration) e CD (Continuous Delivery vs Deployment)
- [ ] Diferença entre Delivery e Deployment: aprovação manual vs automática
- [ ] Por que CI/CD: velocidade, qualidade, redução de risco
- [ ] Pipeline como código: vantagens sobre pipelines clicados em UI
- [ ] Conceito de artefato: o que é, onde guardar (registry, S3, Artifactory)
- [ ] GitFlow vs Trunk-Based Development: impacto no pipeline

## Fase 2 — GitHub Actions (Semanas 2–3)
- [ ] Estrutura do workflow: `on`, `jobs`, `steps`, `runs-on`
- [ ] Triggers: `push`, `pull_request`, `schedule`, `workflow_dispatch`
- [ ] Actions do marketplace vs actions customizadas
- [ ] Secrets e variáveis de ambiente no GitHub Actions
- [ ] Matrix strategy: testar em múltiplas versões/sistemas
- [ ] Cache de dependências (`actions/cache`) para builds mais rápidos
- [ ] Artifacts: salvar e baixar artefatos entre jobs
- [ ] Environments e aprovações manuais para deploy em produção
- [ ] Reusable workflows: compartilhar pipelines entre repositórios
- [ ] Self-hosted runners: quando e como usar

## Fase 3 — Build e Testes no Pipeline (Semana 4)
- [ ] Lint, format check e type check como gates obrigatórios
- [ ] Testes unitários: rodar e publicar relatório de cobertura
- [ ] Testes de integração no CI: subir dependências com `services` (Docker)
- [ ] Análise estática de segurança: SAST (CodeQL, Semgrep)
- [ ] Análise de dependências vulneráveis: Dependabot, `npm audit`
- [ ] Quality gates: bloquear merge se cobertura cair abaixo do threshold
- [ ] Build de imagem Docker no CI com cache de layers

## Fase 4 — Docker e Registry (Semana 5)
- [ ] Build otimizado de imagem Docker: multi-stage build
- [ ] Tagging semântico: `latest`, SHA do commit, semver (`v1.2.3`)
- [ ] Push para Docker Hub, ECR (AWS), GHCR (GitHub)
- [ ] Scan de vulnerabilidades na imagem: Trivy no pipeline
- [ ] Assinatura de imagens: Docker Content Trust / Cosign (Sigstore)
- [ ] Cache de build no registry: `--cache-from` no Docker

## Fase 5 — Deploy Automatizado (Semanas 6–7)
- [ ] Deploy em EC2: SSH + scripts ou AWS CodeDeploy
- [ ] Deploy no ECS (Fargate): atualizar task definition e service
- [ ] Deploy no EKS/Kubernetes: `kubectl set image` ou Helm upgrade
- [ ] Deploy no Lambda: `aws lambda update-function-code`
- [ ] Blue/Green deployment: zero downtime com duas versões paralelas
- [ ] Canary deployment: rolar update para % do tráfego gradualmente
- [ ] Feature flags: desacoplar deploy de release (LaunchDarkly, Flagsmith)
- [ ] Rollback automático: detectar falha e reverter

## Fase 6 — GitOps (Semana 8)
- [ ] O que é GitOps: Git como fonte da verdade da infraestrutura
- [ ] **ArgoCD**: instalação, projetos, sync automático e manual
- [ ] **Flux**: alternativa ao ArgoCD, modelo pull-based
- [ ] Estrutura de repositório GitOps: apps vs infra separados
- [ ] Gerenciar secrets no GitOps: Sealed Secrets, External Secrets Operator
- [ ] Drift detection: detectar diferença entre Git e cluster

## Fase 7 — Ferramentas Complementares e Boas Práticas (Semanas 9–10)
- [ ] **Jenkins**: pipelines declarativos com Jenkinsfile (contexto legado)
- [ ] **GitLab CI**: `.gitlab-ci.yml`, runners, ambientes
- [ ] **AWS CodePipeline + CodeBuild**: pipeline nativo AWS
- [ ] Notificações: Slack, e-mail e PagerDuty no pipeline
- [ ] Métricas de pipeline: DORA metrics (deploy frequency, lead time, MTTR, CFR)
- [ ] Monorepo CI: detectar mudanças por pasta e rodar pipeline seletivo
- [ ] Projeto final: pipeline completo (lint → test → build → scan → deploy → rollback)

## Recursos Recomendados
- Documentação GitHub Actions: https://docs.github.com/actions
- Documentação ArgoCD: https://argo-cd.readthedocs.io
- Livro: "Continuous Delivery" — Jez Humble & David Farley
- Referência DORA: https://dora.dev
