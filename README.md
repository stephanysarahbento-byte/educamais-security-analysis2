# 🔐 EducaMais — Análise de Segurança da Informação

## 📌 Sobre o projeto

A **EducaMais** é uma empresa fictícia do setor de educação que oferece cursos livres por meio de uma plataforma web.

A plataforma permite o cadastro de usuários, realização de pagamentos, acesso a materiais didáticos e acompanhamento do progresso dos alunos.

Com o crescimento da organização, foram identificados problemas relacionados à autenticação, controle de acesso, proteção de dados, monitoramento e gestão de segurança.

Este projeto apresenta uma **análise de Segurança da Informação baseada em riscos**, utilizando boas práticas e referenciais reconhecidos para identificar riscos, priorizar ações e propor controles de segurança.

---

## 🎯 Objetivos

O projeto tem como principais objetivos:

* Identificar ativos e riscos relevantes para a plataforma;
* Avaliar probabilidade e impacto dos riscos;
* Priorizar riscos de acordo com sua criticidade;
* Propor controles técnicos, administrativos e operacionais;
* Estruturar um plano de tratamento de riscos;
* Relacionar os controles aos principais frameworks de segurança;
* Fortalecer a segurança da aplicação web e dos dados dos usuários.

---

## 🚨 Principais riscos identificados

A análise resultou na definição de cinco riscos prioritários:

| ID  | Risco                                       | Probabilidade | Impacto | Prioridade |
| --- | ------------------------------------------- | ------------- | ------- | ---------- |
| R01 | Acesso não autorizado                       | Alta          | Alto    | Crítica    |
| R02 | Exposição de dados sensíveis                | Média         | Alto    | Alta       |
| R03 | Falhas no controle de acesso                | Alta          | Alto    | Crítica    |
| R04 | Ausência de monitoramento e logs            | Média         | Alto    | Alta       |
| R05 | Exploração de vulnerabilidades na aplicação | Alta          | Alto    | Crítica    |

Os riscos relacionados à autenticação, autorização e vulnerabilidades da aplicação receberam maior prioridade devido ao potencial de comprometimento de contas, dados e funcionalidades da plataforma.

---

## 🛡️ Frameworks utilizados

A análise utiliza quatro referências principais:

| Framework                        | Aplicação no projeto                                                                                |
| -------------------------------- | --------------------------------------------------------------------------------------------------- |
| ISO/IEC 27001:2022               | Gestão de riscos, governança e controles de Segurança da Informação                                 |
| NIST Cybersecurity Framework 2.0 | Organização das atividades de governança, identificação, proteção, detecção, resposta e recuperação |
| CIS Controls                     | Implementação de controles técnicos e operacionais priorizados                                      |
| OWASP                            | Identificação e mitigação de riscos relacionados à aplicação web                                    |

Os frameworks são utilizados de forma complementar.

**ISO/IEC 27001 → Governança e Gestão de Riscos**

**NIST CSF → Govern → Identify → Protect → Detect → Respond → Recover**

**CIS Controls → Controles técnicos e operacionais**

**OWASP → Segurança da aplicação web**

---

## 🔐 Principais controles propostos

A partir dos riscos identificados, foram recomendados controles como:

* Autenticação multifator (MFA);
* Políticas de autenticação segura;
* Controle de acesso baseado em funções (RBAC);
* Princípio do menor privilégio;
* Revisão periódica de permissões;
* Criptografia de dados sensíveis;
* Proteção de dados em trânsito;
* Registro e centralização de logs;
* Monitoramento e alertas de segurança;
* Gestão contínua de vulnerabilidades;
* Atualização de bibliotecas e componentes;
* Testes de segurança da aplicação;
* Desenvolvimento seguro;
* Backups periódicos;
* Procedimentos de resposta a incidentes.

---

## 🚦 Estratégia de implementação

Os controles foram organizados em três fases.

### Fase 1 — Controles prioritários

* Implementação de MFA;
* Controle de acesso baseado em funções;
* Princípio do menor privilégio;
* Correção de vulnerabilidades críticas;
* Implementação de logs de segurança.

### Fase 2 — Fortalecimento da segurança

* Criptografia de dados sensíveis;
* Monitoramento contínuo;
* Alertas de segurança;
* Revisão periódica de permissões;
* Gestão de vulnerabilidades.

### Fase 3 — Melhoria contínua

* Avaliações periódicas de riscos;
* Testes de segurança;
* Revisão dos controles;
* Atualização de sistemas e componentes;
* Simulação e tratamento de incidentes.

---

## 📊 Indicadores de segurança

Para acompanhar a efetividade dos controles, foram definidos indicadores como:

* Percentual de contas protegidas por MFA;
* Número de tentativas de acesso bloqueadas;
* Número de vulnerabilidades críticas abertas;
* Tempo médio para correção de vulnerabilidades;
* Número de incidentes detectados;
* Tempo médio de resposta a incidentes;
* Percentual de acessos e privilégios revisados.

---

## 📂 Estrutura do projeto

```text
educamais-security-analysis2/
│
├── docs/
│   ├── analise-riscos.md
│   ├── gestao-de-riscos.md
│   ├── plano-de-tratamento.md
│   ├── iso-27001.md
│   ├── nist-csf.md
│   ├── cis-controls.md
│   └── owasp.md
│
├── diagrams/
│   └── documentação visual da arquitetura de segurança
│
└── README.md
```

---

## 📚 Documentação

### Gestão de riscos

* [Análise de Riscos](docs/analise-riscos.md)
* [Gestão de Riscos](docs/gestao-de-riscos.md)
* [Plano de Tratamento de Riscos](docs/plano-de-tratamento.md)

### Frameworks

* [ISO/IEC 27001](docs/iso-27001.md)
* [NIST Cybersecurity Framework](docs/nist-csf.md)
* [CIS Controls](docs/cis-controls.md)
* [OWASP](docs/owasp.md)

### Arquitetura

Os diagramas do projeto estão disponíveis no diretório [`diagrams/`](diagrams/).

---

## 🔄 Fluxo da análise

O projeto segue uma abordagem estruturada:

**Contexto → Identificação de Ativos → Identificação de Riscos → Avaliação → Priorização → Tratamento → Monitoramento → Melhoria Contínua**

Essa abordagem permite relacionar os problemas identificados aos riscos, controles e ações de tratamento.

---

## 🎯 Resultado esperado

Com a implementação das medidas propostas, espera-se:

* Redução da probabilidade de comprometimento de contas;
* Maior proteção dos dados dos usuários;
* Redução de privilégios excessivos;
* Maior segurança da aplicação web;
* Maior capacidade de detecção de atividades suspeitas;
* Melhoria da resposta a incidentes;
* Fortalecimento da gestão de vulnerabilidades;
* Evolução da maturidade de Segurança da Informação.

---

## 📝 Conclusão

A análise da EducaMais demonstra que a Segurança da Informação deve envolver não apenas controles técnicos, mas também gestão de riscos, governança, monitoramento e melhoria contínua.

A utilização integrada da **ISO/IEC 27001:2022, NIST CSF 2.0, CIS Controls e OWASP** permite abordar os riscos sob diferentes perspectivas, combinando governança, gestão, controles técnicos e segurança de aplicações.

O projeto demonstra a aplicação prática de conceitos de **análise de riscos, controle de acesso, proteção de dados, gestão de vulnerabilidades, monitoramento e resposta a incidentes** em um cenário corporativo fictício.

---

## 📚 Referenciais

* ISO/IEC 27001:2022
* NIST Cybersecurity Framework 2.0
* CIS Controls
* OWASP

---

**Projeto acadêmico — Segurança da Informação**

**Empresa analisada:** EducaMais
**Status:** Concluído
