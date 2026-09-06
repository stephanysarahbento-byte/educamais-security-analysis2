# Gestão de Riscos de Segurança da Informação — EducaMais

## 1. Objetivo

Este documento apresenta a identificação, análise e avaliação dos principais riscos de Segurança da Informação relacionados à plataforma EducaMais.

A gestão de riscos tem como objetivo identificar eventos que possam comprometer a **confidencialidade, integridade e disponibilidade das informações**, permitindo a definição de controles e ações para reduzir os riscos a níveis aceitáveis.

A análise foi estruturada com base em boas práticas de Segurança da Informação e em referências como:

* ISO/IEC 27001;
* NIST Cybersecurity Framework (CSF) 2.0;
* CIS Controls;
* OWASP.

---

# 2. Metodologia de Avaliação de Riscos

Os riscos foram avaliados considerando dois fatores principais:

* **Probabilidade:** possibilidade de ocorrência do evento;
* **Impacto:** consequência para a organização caso o evento ocorra.

A classificação do risco é obtida pela combinação entre probabilidade e impacto.

## Escala de Probabilidade

| Classificação | Descrição                                          |
| ------------- | -------------------------------------------------- |
| Baixa         | Evento pouco provável de ocorrer                   |
| Média         | Evento pode ocorrer em determinadas circunstâncias |
| Alta          | Evento possui grande possibilidade de ocorrer      |

## Escala de Impacto

| Classificação | Descrição                                                   |
| ------------- | ----------------------------------------------------------- |
| Baixo         | Impacto limitado para a operação                            |
| Médio         | Impacto relevante para usuários ou operação                 |
| Alto          | Impacto significativo para a organização, dados ou serviços |

## Níveis de Risco

| Probabilidade | Impacto | Nível de Risco |
| ------------- | ------- | -------------- |
| Baixa         | Baixo   | Baixo          |
| Média         | Médio   | Médio          |
| Alta          | Alto    | Alto           |
| Média         | Alto    | Alto           |
| Alta          | Médio   | Alto           |

---

# 3. Ativos Identificados

Os principais ativos relacionados à plataforma EducaMais incluem:

| Ativo                   | Descrição                                       |
| ----------------------- | ----------------------------------------------- |
| Plataforma Web          | Aplicação utilizada pelos usuários da EducaMais |
| Dados dos Usuários      | Informações pessoais e dados cadastrais         |
| Banco de Dados          | Armazenamento das informações da plataforma     |
| Sistema de Autenticação | Responsável pela validação dos usuários         |
| Contas Administrativas  | Contas com privilégios elevados                 |
| Infraestrutura          | Servidores, serviços e recursos tecnológicos    |
| Logs                    | Registros de eventos e atividades da plataforma |

---

# 4. Riscos Identificados

## Risco 01 — Acesso não autorizado

### Descrição

Usuários não autorizados podem obter acesso à plataforma ou a informações restritas devido a falhas nos mecanismos de autenticação ou controle de acesso.

### Ativos afetados

* Dados dos usuários;
* Contas administrativas;
* Plataforma Web.

### Ameaças

* Roubo de credenciais;
* Ataques de força bruta;
* Credenciais comprometidas;
* Acessos indevidos.

### Vulnerabilidades

* Senhas fracas;
* Ausência de autenticação multifator;
* Falhas no controle de acesso.

### Avaliação

| Probabilidade | Impacto | Nível de Risco |
| ------------- | ------- | -------------- |
| Alta          | Alto    | Alto           |

### Controles recomendados

* Implementação de MFA;
* Política de senhas fortes;
* Controle de acesso baseado em perfis;
* Princípio do menor privilégio;
* Monitoramento de tentativas de autenticação.

---

# 5. Risco 02 — Exposição de Dados Sensíveis

## Descrição

Informações pessoais ou sensíveis podem ser acessadas, expostas ou divulgadas sem autorização.

### Ativos afetados

* Dados dos usuários;
* Banco de dados;
* Informações cadastrais.

### Ameaças

* Vazamento de dados;
* Ataques à aplicação;
* Acesso indevido ao banco de dados.

### Vulnerabilidades

* Ausência de criptografia;
* Configurações incorretas;
* Controle de acesso inadequado.

### Avaliação

| Probabilidade | Impacto | Nível de Risco |
| ------------- | ------- | -------------- |
| Média         | Alto    | Alto           |

### Controles recomendados

* Criptografia de dados;
* Controle de acesso;
* Classificação das informações;
* Monitoramento de acessos;
* Revisão de permissões.

---

# 6. Risco 03 — Falhas no Controle de Acesso

## Descrição

Usuários podem acessar recursos ou funcionalidades para os quais não possuem autorização.

### Ativos afetados

* Plataforma Web;
* Contas administrativas;
* Dados dos usuários.

### Ameaças

* Escalonamento de privilégios;
* Acesso indevido a funcionalidades;
* Manipulação de permissões.

### Vulnerabilidades

* Falhas na implementação de autorização;
* Permissões excessivas;
* Ausência de validação de privilégios.

### Avaliação

| Probabilidade | Impacto | Nível de Risco |
| ------------- | ------- | -------------- |
| Alta          | Alto    | Alto           |

### Controles recomendados

* Controle de acesso baseado em funções;
* Princípio do menor privilégio;
* Revisão periódica de permissões;
* Validação de autorização no servidor.

---

# 7. Risco 04 — Ausência de Monitoramento e Logs

## Descrição

A ausência ou insuficiência de registros de eventos pode dificultar a identificação e investigação de incidentes de segurança.

### Ativos afetados

* Plataforma Web;
* Infraestrutura;
* Dados dos usuários.

### Ameaças

* Atividades maliciosas não detectadas;
* Incidentes não identificados;
* Dificuldade na investigação de eventos.

### Vulnerabilidades

* Ausência de logs;
* Monitoramento insuficiente;
* Falta de alertas de segurança.

### Avaliação

| Probabilidade | Impacto | Nível de Risco |
| ------------- | ------- | -------------- |
| Média         | Alto    | Alto           |

### Controles recomendados

* Registro de eventos;
* Centralização de logs;
* Monitoramento contínuo;
* Alertas de segurança;
* Procedimentos de resposta a incidentes.

---

# 8. Risco 05 — Exploração de Vulnerabilidades na Aplicação

## Descrição

Vulnerabilidades presentes na aplicação podem ser exploradas por atacantes, comprometendo sistemas, informações ou usuários.

### Ativos afetados

* Plataforma Web;
* Banco de Dados;
* Dados dos usuários.

### Ameaças

* Exploração de vulnerabilidades;
* Ataques a aplicações web;
* Execução de ações não autorizadas.

### Vulnerabilidades

* Falhas de desenvolvimento seguro;
* Bibliotecas desatualizadas;
* Validação inadequada de entradas.

### Avaliação

| Probabilidade | Impacto | Nível de Risco |
| ------------- | ------- | -------------- |
| Alta          | Alto    | Alto           |

### Controles recomendados

* Desenvolvimento seguro;
* Análise de vulnerabilidades;
* Atualização de componentes;
* Validação de entradas;
* Testes de segurança.

---

# 9. Matriz Consolidada de Riscos

| ID  | Risco                            | Probabilidade | Impacto | Nível |
| --- | -------------------------------- | ------------- | ------- | ----- |
| R01 | Acesso não autorizado            | Alta          | Alto    | Alto  |
| R02 | Exposição de dados sensíveis     | Média         | Alto    | Alto  |
| R03 | Falhas no controle de acesso     | Alta          | Alto    | Alto  |
| R04 | Ausência de monitoramento e logs | Média         | Alto    | Alto  |
| R05 | Exploração de vulnerabilidades   | Alta          | Alto    | Alto  |

---

# 10. Relação com Frameworks de Segurança

Os riscos identificados podem ser tratados utilizando práticas e controles recomendados pelos principais frameworks de Segurança da Informação.

| Framework     | Aplicação                                                                |
| ------------- | ------------------------------------------------------------------------ |
| ISO/IEC 27001 | Gestão de riscos e implementação de controles de Segurança da Informação |
| NIST CSF 2.0  | Identificação, proteção, detecção, resposta e recuperação                |
| CIS Controls  | Implementação de controles técnicos e operacionais priorizados           |
| OWASP         | Identificação e mitigação de riscos relacionados a aplicações web        |

---

# 11. Conclusão

A análise identificou riscos relevantes relacionados principalmente à autenticação, controle de acesso, proteção de dados, monitoramento e segurança da aplicação.

Os riscos classificados como altos devem receber prioridade no plano de tratamento. A implementação dos controles recomendados pode reduzir a probabilidade de incidentes e minimizar seus impactos.

A gestão de riscos deve ser um processo contínuo, com revisões periódicas dos ativos, ameaças, vulnerabilidades e controles implementados.
