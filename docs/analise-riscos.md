# Análise de Riscos — EducaMais

## 1. Contexto

A EducaMais é uma empresa fictícia do setor de educação que oferece cursos livres por meio de uma plataforma web.

A plataforma realiza cadastro de usuários, pagamentos, disponibilização de materiais didáticos e acompanhamento do progresso dos alunos.

O crescimento acelerado da empresa ocorreu sem a evolução proporcional dos controles de segurança da informação, aumentando a exposição da organização a riscos relacionados à confidencialidade, integridade e disponibilidade das informações.

---

## 2. Principais riscos identificados

A análise inicial permitiu identificar cinco riscos prioritários para a plataforma EducaMais.

| ID  | Risco                                       | Impacto | Probabilidade | Prioridade |
| --- | ------------------------------------------- | ------- | ------------- | ---------- |
| R01 | Acesso não autorizado                       | Alto    | Alta          | Crítica    |
| R02 | Exposição de dados sensíveis                | Alto    | Média         | Alta       |
| R03 | Falhas no controle de acesso                | Alto    | Alta          | Crítica    |
| R04 | Ausência de monitoramento e logs            | Alto    | Média         | Alta       |
| R05 | Exploração de vulnerabilidades na aplicação | Alto    | Alta          | Crítica    |

Os riscos relacionados à autenticação, autorização e exploração de vulnerabilidades recebem maior prioridade devido ao potencial de comprometimento de contas, dados e funcionalidades da plataforma.

---

## 3. Direcionamento para tratamento dos riscos

O tratamento deve priorizar inicialmente os riscos classificados como críticos, especialmente aqueles relacionados a autenticação, controle de acesso e vulnerabilidades da aplicação.

Entre as principais medidas recomendadas estão:

* implementação de autenticação multifator (MFA);
* fortalecimento das políticas de autenticação;
* adoção do princípio do menor privilégio;
* controle de acesso baseado em funções;
* revisão periódica de permissões;
* proteção e criptografia de dados;
* registro e centralização de logs;
* monitoramento de eventos de segurança;
* gestão contínua de vulnerabilidades;
* testes de segurança na aplicação;
* estabelecimento de procedimentos de resposta a incidentes.

O detalhamento das ações de mitigação é apresentado no documento `plano-de-tratamento.md`.

---

## 4. Referenciais utilizados

A análise utiliza como referências:

* ISO/IEC 27001:2022;
* NIST Cybersecurity Framework (CSF) 2.0;
* CIS Controls;
* OWASP.

Esses referenciais são utilizados de forma complementar para apoiar a gestão de riscos, a implementação de controles de segurança, a proteção da aplicação web e a melhoria contínua da postura de segurança da EducaMais.

---

## 5. Relação com a Gestão de Riscos

Este documento apresenta uma visão resumida dos principais riscos identificados na EducaMais.

A análise detalhada dos ativos, ameaças, vulnerabilidades, probabilidade, impacto e controles recomendados está disponível no documento `gestao-de-riscos.md`.

As ações definidas para mitigação e acompanhamento dos riscos estão documentadas em `plano-de-tratamento.md`.

Dessa forma, os documentos formam um fluxo integrado de análise e tratamento:

**Análise de Riscos → Gestão de Riscos → Plano de Tratamento**
