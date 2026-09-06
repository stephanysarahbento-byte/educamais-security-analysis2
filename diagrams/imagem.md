# Diagrama de Segurança — EducaMais

Este documento apresenta uma visão geral da estrutura de Segurança da Informação do projeto EducaMais e a integração dos principais frameworks utilizados na análise.

## Arquitetura da Segurança

```mermaid
flowchart TB

    A[EducaMais<br/>Plataforma de Educação Online]

    A --> B[Plataforma Web]

    B --> C[Alunos]
    B --> D[Administradores]
    B --> E[Pagamentos]
    B --> F[Materiais Didáticos]

    A --> G[Programa de Segurança da Informação]

    G --> H[ISO/IEC 27001:2022]
    G --> I[NIST CSF 2.0]
    G --> J[CIS Controls]
    G --> K[OWASP]

    H --> H1[Governança]
    H --> H2[Gestão de Riscos]

    I --> I1[Govern]
    I --> I2[Identify]
    I --> I3[Protect]
    I --> I4[Detect]
    I --> I5[Respond]
    I --> I6[Recover]

    J --> J1[Gestão de Ativos]
    J --> J2[Controle de Acesso]
    J --> J3[Gestão de Vulnerabilidades]

    K --> K1[Autenticação]
    K --> K2[Controle de Acesso]
    K --> K3[Desenvolvimento Seguro]

    G --> L[Riscos Identificados]

    L --> L1[Acessos não autorizados]
    L --> L2[Falhas de autenticação]
    L --> L3[Privilégios excessivos]
    L --> L4[Ausência de monitoramento]

    G --> M[Controles de Segurança]

    M --> M1[MFA]
    M --> M2[Menor Privilégio]
    M --> M3[Logs e Monitoramento]
    M --> M4[Gestão de Vulnerabilidades]
    M --> M5[Resposta a Incidentes]