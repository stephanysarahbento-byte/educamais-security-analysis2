# OWASP — Segurança da Aplicação Web da EducaMais

## 1. Visão geral

A OWASP fornece boas práticas e referências voltadas à segurança de aplicações web.

Esse referencial é especialmente importante para a EducaMais porque os principais problemas identificados estão relacionados à plataforma web, principalmente aos mecanismos de login, redefinição de senha e controle de acesso.

## 2. Autenticação

O mecanismo de login deve ser protegido contra ataques que possam comprometer as contas dos usuários.

Entre as medidas recomendadas estão:

- Uso de senhas fortes;
- Proteção contra tentativas automatizadas;
- MFA para contas administrativas;
- Controle adequado de sessões;
- Proteção das credenciais;
- Monitoramento de tentativas de autenticação.

### Aplicação na EducaMais

Como foram identificados acessos não autorizados e falhas no formulário de login, a autenticação deve ser tratada como uma das prioridades de segurança.

## 3. Redefinição de senha

O processo de recuperação de senha deve utilizar mecanismos seguros.

Os tokens de recuperação devem ser:

- Imprevisíveis;
- De uso limitado;
- Com validade limitada;
- Invalidados após a utilização.

### Aplicação na EducaMais

As falhas identificadas no módulo de redefinição de senha podem permitir comprometimento de contas. Por isso, esse mecanismo deve ser revisado e testado prioritariamente.

## 4. Controle de acesso

Os usuários devem ter acesso somente aos recursos necessários para suas funções.

A aplicação deve verificar as permissões no servidor e não apenas na interface.

### Aplicação na EducaMais

Esse controle é especialmente importante porque foram identificados colaboradores com privilégios administrativos acima do necessário.

Além disso, alunos não devem conseguir acessar informações de outros usuários ou funções administrativas.

## 5. Proteção contra vulnerabilidades

A aplicação deve passar por processos contínuos de identificação e correção de vulnerabilidades.

Entre as práticas recomendadas estão:

- Testes de segurança;
- Code review;
- Análise de dependências;
- Correção de vulnerabilidades;
- Atualização de componentes;
- Proteção de informações sensíveis.

## 6. Desenvolvimento seguro

A segurança deve fazer parte de todo o ciclo de desenvolvimento:

**Requisitos → Desenvolvimento → Code Review → Testes → Deploy → Monitoramento**

Essa abordagem reduz a possibilidade de vulnerabilidades chegarem ao ambiente de produção.

## 7. Disponibilidade e abuso de requisições

A instabilidade apresentada após o aumento repentino de requisições demonstra a necessidade de avaliar a capacidade da aplicação de lidar com picos de acesso e possíveis comportamentos abusivos.

Entre as medidas que podem ser avaliadas estão:

- Rate limiting;
- Monitoramento de tráfego;
- Proteção contra abuso de requisições;
- Testes de carga;
- Monitoramento da disponibilidade.

## 8. Justificativa

A OWASP complementa os demais frameworks com uma visão técnica específica sobre aplicações web.

Enquanto a ISO 27001 trata da gestão e governança, o NIST CSF organiza o ciclo de segurança e os CIS Controls apresentam ações práticas, a OWASP permite aprofundar a análise dos riscos diretamente relacionados à plataforma web da EducaMais.

## 9. Relação com os demais frameworks

A ISO 27001 fornece a estrutura de gestão e governança.

O NIST CSF organiza as atividades de segurança.

Os CIS Controls apresentam controles práticos e priorizados.

A OWASP direciona a aplicação dessas práticas para os riscos específicos da plataforma web.
