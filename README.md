# 🔐 EducaMais — Análise de Segurança da Informação

## 📌 Sobre o projeto

A **EducaMais** é uma empresa fictícia do setor de educação que oferece cursos livres por meio de uma plataforma web.

A plataforma permite que os alunos realizem cadastro, efetuem pagamentos, acessem materiais didáticos e acompanhem seu progresso em ambiente online.

Com o crescimento acelerado da empresa, foram identificados problemas relacionados à segurança da informação.

Este projeto apresenta uma análise inicial desses problemas e propõe medidas de segurança com base em frameworks e boas práticas reconhecidas.

---

## 🚨 Problemas identificados

Foram identificados os seguintes problemas:

- 🔴 Acessos não autorizados em contas de usuários;
- 🔴 Falhas no formulário de login;
- 🔴 Falhas no módulo de redefinição de senha;
- 🟠 Instabilidade após aumento de requisições;
- 🔴 Privilégios administrativos acima do necessário;
- 🟠 Ausência de processo formal de gestão de riscos;
- 🟠 Ausência de processo definido de resposta a incidentes;
- 🟡 Baixa conscientização dos colaboradores.

---

## 🎯 Objetivos

O projeto tem como objetivos:

- Identificar os principais riscos de segurança;
- Priorizar controles e ações;
- Analisar os riscos da plataforma web;
- Propor medidas de prevenção e proteção;
- Estruturar uma abordagem de resposta a incidentes;
- Integrar diferentes frameworks de segurança.

---

## 🛡️ Frameworks utilizados

A análise utiliza quatro referências principais:

| Framework | Principal contribuição |
|---|---|
| ISO/IEC 27001:2022 | Gestão e governança da segurança |
| NIST CSF 2.0 | Gestão do ciclo de segurança cibernética |
| CIS Controls | Controles e ações práticas de segurança |
| OWASP | Segurança de aplicações web |

---

## 1. ISO/IEC 27001:2022

A ISO/IEC 27001:2022 fornece uma estrutura para estabelecer e manter um Sistema de Gestão de Segurança da Informação (SGSI) baseado em riscos.

### Aplicação na EducaMais

A empresa deve:

- Identificar e avaliar riscos;
- Definir políticas de segurança;
- Estabelecer responsabilidades;
- Implementar controles;
- Monitorar os resultados;
- Promover melhoria contínua.

### Justificativa

A EducaMais não possui um processo formal de gestão de riscos. Portanto, a ISO 27001 é importante para transformar a segurança em um processo contínuo de gestão, e não apenas em ações pontuais após a ocorrência de problemas.

---

## 2. NIST Cybersecurity Framework 2.0

O NIST CSF 2.0 organiza a segurança cibernética em seis funções:

```text
Govern
   ↓
Identify
   ↓
Protect
   ↓
Detect
   ↓
Respond
   ↓
Recover
