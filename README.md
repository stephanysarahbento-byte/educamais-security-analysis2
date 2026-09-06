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
### Aplicação na EducaMais
Govern: estabelecer políticas, responsabilidades e critérios de risco.

Identify: identificar ativos, sistemas, dados e riscos.

Protect: implementar MFA, controle de acesso, proteção de dados e autenticação adequada.

Detect: monitorar logs e identificar atividades suspeitas.

Respond: estabelecer procedimentos para tratar incidentes.

Recover: implementar backups e procedimentos de recuperação.

Justificativa
O NIST CSF permite organizar a segurança como um ciclo contínuo, desde a identificação dos riscos até a recuperação após um incidente.

3. CIS Controls
Os CIS Controls apresentam práticas de segurança que podem ser utilizadas de forma prática e priorizada.

Aplicação na EducaMais
Entre as principais ações estão:

Inventário de ativos;
Gerenciamento de contas;
Controle de acesso;
Gestão de vulnerabilidades;
Configuração segura;
Gerenciamento de logs;
Proteção de dados;
Monitoramento;
Conscientização dos colaboradores;
Resposta a incidentes.
Justificativa
Os CIS Controls complementam os demais frameworks ao transformar objetivos de segurança em ações práticas.

No caso da EducaMais, são especialmente importantes para tratar os privilégios excessivos, as vulnerabilidades e o monitoramento do ambiente.

4. OWASP
A OWASP é especialmente relevante porque a EducaMais possui uma plataforma web.

Principais pontos de atenção
🔑 Autenticação
O mecanismo de login deve ser protegido contra tentativas automatizadas, abuso de credenciais e outros ataques.

🔄 Redefinição de senha
O mecanismo de recuperação deve utilizar tokens seguros, imprevisíveis e com validade limitada.

👤 Controle de acesso
Cada usuário deve acessar somente os recursos para os quais possui autorização.

Um aluno, por exemplo, não deve conseguir acessar informações de outro aluno ou funções administrativas.

💻 Desenvolvimento seguro
A segurança deve fazer parte de todo o ciclo de desenvolvimento:
Requisitos
    ↓
Desenvolvimento
    ↓
Code Review
    ↓
Testes de Segurança
    ↓
Deploy
    ↓
Monitoramento

Justificativa
A OWASP complementa os demais referenciais com uma visão técnica sobre os riscos específicos da aplicação web.

🔗 Integração dos frameworks
Os quatro referenciais devem ser utilizados de maneira complementar.
                 EDUCAMais
                     │
                     ▼
              Gestão de Riscos
                     │
        ┌────────────┼────────────┐
        ▼            ▼            ▼
   ISO 27001      NIST CSF    CIS Controls
   Governança      Ciclo      Ações práticas
        │            │            │
        └────────────┼────────────┘
                     ▼
                   OWASP
                     │
                     ▼
          Segurança da aplicação

A ISO 27001 fornece a visão de gestão e governança.

O NIST CSF organiza o ciclo de segurança.

Os CIS Controls apresentam ações práticas e priorizadas.

A OWASP aprofunda a segurança da aplicação web.

🚦 Priorização das ações
🔴 Prioridade 1 — Riscos críticos
Corrigir vulnerabilidades no login;
Corrigir a redefinição de senha;
Revisar privilégios administrativos;
Implementar MFA para contas administrativas;
Investigar acessos não autorizados;
Analisar logs;
Corrigir vulnerabilidades críticas da aplicação.
🟠 Prioridade 2 — Detecção e resposta
Criar processo de resposta a incidentes;
Definir responsáveis;
Implementar monitoramento;
Criar procedimentos de contenção;
Estabelecer canais de comunicação.
🟡 Prioridade 3 — Governança
Criar política de segurança;
Realizar inventário de ativos;
Criar registro de riscos;
Definir responsáveis pelos riscos;
Estabelecer indicadores.
🟢 Prioridade 4 — Desenvolvimento seguro
Code review;
Testes de segurança;
Análise de dependências;
Gestão de vulnerabilidades;
Proteção de segredos;
Testes de autenticação e autorização.
🔵 Prioridade 5 — Pessoas
Treinamento de segurança;
Conscientização sobre phishing;
Boas práticas de senhas;
Uso correto de MFA;
Proteção de dados;
Comunicação de incidentes.

## 📊 Plano de ação

| Prazo | Ação | Referencial |
|---|---|---|
| Imediato | Corrigir login e recuperação de senha | OWASP |
| Imediato | Revisar privilégios administrativos | CIS / OWASP |
| Imediato | Proteger contas administrativas com MFA | NIST / CIS |
| Imediato | Investigar acessos não autorizados | NIST |
| Curto prazo | Implantar logs e monitoramento | NIST / CIS |
| Curto prazo | Criar resposta a incidentes | NIST / ISO 27001 |
| Curto prazo | Inventariar ativos | CIS / ISO 27001 |
| Médio prazo | Estruturar gestão de riscos | ISO 27001 |
| Médio prazo | Implementar desenvolvimento seguro | OWASP |
| Contínuo | Treinar colaboradores | ISO / NIST / CIS |
| Contínuo | Revisar e melhorar os controles | ISO 27001 |

🎯 Resultado esperado
Com a implementação das medidas propostas, espera-se:

Redução do risco de comprometimento de contas;
Redução de privilégios excessivos;
Maior proteção da aplicação web;
Maior capacidade de detectar ataques;
Resposta mais rápida a incidentes;
Maior disponibilidade da plataforma;
Melhoria da cultura de segurança;
Estrutura formal de gestão de riscos.
📝 Conclusão
Os problemas encontrados na EducaMais não representam apenas falhas técnicas. Eles demonstram uma baixa maturidade geral em segurança da informação.

A integração entre ISO 27001, NIST CSF, CIS Controls e OWASP permite abordar o problema de forma abrangente.

A ISO 27001 fornece a estrutura de gestão e governança; o NIST CSF organiza o ciclo de segurança; os CIS Controls apresentam ações práticas; e a OWASP fornece uma visão específica sobre a segurança da aplicação web.

Dessa forma, a EducaMais pode evoluir de uma postura reativa para uma abordagem estruturada, baseada em riscos e orientada à melhoria contínua.

📚 Referenciais
ISO/IEC 27001:2022
NIST Cybersecurity Framework 2.0
CIS Controls
OWASP
Projeto acadêmico — Segurança da Informação

Empresa: EducaMais
Status: Análise inicial