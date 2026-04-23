# Linha do Tempo de Estudos — DevOps

## Fase 1 — Cultura e Fundamentos (Semana 1)
- [ ] O que é DevOps: cultura, não ferramenta
- [ ] Os três caminhos do DevOps: Fluxo, Feedback e Aprendizado Contínuo
- [ ] DevOps vs SRE vs Platform Engineering: diferenças e sobreposições
- [ ] CALMS: Culture, Automation, Lean, Measurement, Sharing
- [ ] DORA Metrics: as 4 métricas que importam para medir maturidade DevOps
- [ ] Identificar silos entre Dev e Ops: como e por que quebrá-los
- [ ] Blameless postmortem: cultura de aprendizado sem punição

## Fase 2 — Controle de Versão e Colaboração (Semana 2)
- [ ] Git avançado: rebase, cherry-pick, stash, bisect
- [ ] Estratégias de branching: GitFlow, GitHub Flow, Trunk-Based Development
- [ ] Conventional Commits: padronizar mensagens de commit
- [ ] Semantic Versioning (SemVer): `MAJOR.MINOR.PATCH`
- [ ] Pull Request como processo: revisão de código, templates, checks obrigatórios
- [ ] Monorepo vs Polyrepo: trade-offs para times grandes
- [ ] Inner Source: práticas open source dentro da empresa

## Fase 3 — Linux e Shell para DevOps (Semanas 3–4)
- [ ] Filesystem Linux: FHS, permissões, links simbólicos
- [ ] Gerenciamento de processos: `systemd`, `journalctl`, `top`, `htop`
- [ ] Shell scripting Bash: variáveis, loops, condicionais, funções
- [ ] Pipelines de texto: `grep`, `awk`, `sed`, `sort`, `uniq`, `cut`
- [ ] Networking: `netstat`, `ss`, `curl`, `wget`, `tcpdump`, `nmap`
- [ ] SSH: chaves, tunneling, ProxyJump, `~/.ssh/config`
- [ ] Cron e agendamento de tarefas
- [ ] Gerenciamento de pacotes: `apt`, `yum`, `snap`

## Fase 4 — Containers (Semana 5)
- [ ] Como containers funcionam: namespaces e cgroups do Linux
- [ ] Docker: imagens, containers, volumes, networks
- [ ] Dockerfile: instrução por instrução, multi-stage builds
- [ ] Docker Compose: orquestrar serviços em desenvolvimento
- [ ] Docker Hub e registries privados
- [ ] Segurança em containers: usuário não-root, imagens mínimas (distroless/alpine)
- [ ] Diferença entre VM e container: casos de uso de cada um

## Fase 5 — Infraestrutura como Código (Semana 6)
- [ ] Princípios de IaC: idempotência, declarativo vs imperativo
- [ ] Terraform: conceitos, state, módulos (ver arquivo terraform.md)
- [ ] Ansible: playbooks, roles, inventários, idempotência
- [ ] Diferença entre Terraform (provisioning) e Ansible (configuration management)
- [ ] Packer: criar AMIs e imagens customizadas
- [ ] Immutable infrastructure: rebake em vez de patch

## Fase 6 — Observabilidade (Semanas 7–8)
- [ ] Os três pilares: Logs, Métricas e Traces
- [ ] **Logs estruturados**: JSON logs, níveis (DEBUG/INFO/WARN/ERROR)
- [ ] Stack ELK/EFK: Elasticsearch, Logstash/Fluentd, Kibana
- [ ] **Métricas**: Prometheus + Grafana, alertas com Alertmanager
- [ ] **Tracing distribuído**: OpenTelemetry, Jaeger
- [ ] APM: Application Performance Monitoring (Datadog, New Relic)
- [ ] SLI, SLO e SLA: definir e monitorar indicadores de serviço
- [ ] Error budget: o quanto de falha é aceitável por período
- [ ] On-call e runbooks: como documentar e responder a incidentes

## Fase 7 — Segurança (DevSecOps) (Semana 9)
- [ ] Shift-left security: trazer segurança para o início do ciclo
- [ ] SAST (Static Analysis): análise de código fonte (SonarQube, Semgrep)
- [ ] DAST (Dynamic Analysis): testes em aplicação rodando (OWASP ZAP)
- [ ] Gerenciamento de secrets: Vault, AWS Secrets Manager
- [ ] Princípio do menor privilégio em IAM
- [ ] Compliance como código: Open Policy Agent, Checkov
- [ ] Threat modeling: identificar riscos antes de codar

## Fase 8 — Platform Engineering e Maturidade (Semana 10)
- [ ] Internal Developer Platform (IDP): abstrair complexidade para devs
- [ ] Backstage (Spotify): portal do desenvolvedor
- [ ] Golden paths: caminhos padrão e aprovados para times
- [ ] FinOps: custo de cloud como métrica de engenharia
- [ ] Chaos Engineering: Chaos Monkey, Gremlin, LitmusChaos
- [ ] Roadmap de maturidade DevOps: onde você está, para onde ir
- [ ] Projeto final: mapear e apresentar a evolução DevOps de um projeto real

## Recursos Recomendados
- Livro: "The Phoenix Project" — Gene Kim (narrativa, leitura obrigatória)
- Livro: "The DevOps Handbook" — Gene Kim et al.
- Livro: "Site Reliability Engineering" — Google (gratuito online)
- Certificação: AWS DevOps Engineer Professional
- Referência DORA: https://dora.dev
