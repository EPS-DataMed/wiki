<br/>

<div style="display: flex; flex-direction: column; justify-content: center; align-items:center;">
    <img src="https://dansousamelo.github.io/RQ_ISP/assets/ARQ01.png" width="200" height="200" style="filter: brightness(0%);" />
</div>

<br/>

## Histórico de versões

| Versão |    Data    |              Descrição               |                      Autor(es)                       | Revisor(es) |
| :----: | :--------: | :----------------------------------: | :--------------------------------------------------: | :---------: |
| `1.0`  | 24/04/2024 | Criando documento de Tecnologias | Todos do grupo|      -      |

## 1. Introdução

### 1.1 Objetivo do Documento
Este documento tem como objetivo oferecer uma visão técnica e outras abordagens da **arquitetura** do sistema **Datamed**, que viabiliza o **cadastro de usuários** (comuns e médicos), a **submissão de exames**, a gestão de **dependentes/pacientes** e a geração de **cartões com informações dos exames** para impressão.

### 1.2 Escopo do Sistema
O escopo do sistema **Datamed** abrange:
- **Front-end**: Desenvolvido com **React.js**, **jest** e **TypeScript**.
- **Microserviços**: Implementado com **FastAPI**, **Python** e **pytest**.
- **Banco de dados**: **PostgreSQL**.
- **Ambientes de produção**: **Render**.


## 2. Padrões e Convenções
**Padrões Arquitetônicos Utilizados**

- Arquitetura de **microsserviços** para o **back-end**.
- Componentização no **front-end** com **React**.

**Convenções de Codificação**

- Seguir padrões de codificação do **PEP 8** para **Python**.
- Utilizar **ESLint** e **Prettier** para manter a consistência do código no **front-end**.

## 3. Decisões Arquitetônicas
**Principais Decisões e Justificativas**

- Escolha de **React.js** e **TypeScript** para robustez e escalabilidade do **front-end**.
- Utilização de **FastAPI** e **Python** no **back-end** pela facilidade de desenvolvimento rápido e integração com bibliotecas de processamento de dados.
- Uso de **PostgreSQL** devido à sua robustez e suporte a transações complexas.
- Adoção de uma arquitetura de **microsserviços** para facilitar a escalabilidade e manutenção do sistema.

**Trade-offs Considerados**

- Escolha entre **FastAPI** e **Django**, optando por **FastAPI** pela performance e simplicidade.
- Escolha entre **PostgreSQL** e **MySQL**, optando por **PostgreSQL** pela melhor conformidade com **ACID**.

## 4. Segurança
**Mecanismos de Segurança Implementados**

- Autenticação baseada em **JWT**.
- Criptografia de senhas.
- Conexões **HTTPS** para comunicação segura.

**Políticas de Segurança**

- Políticas de controle de acesso baseadas em papéis (**RBAC**).
- Auditoria e logs de atividades.


## Referências
- FOWLER, Martin. Patterns of Enterprise Application Architecture. Addison-Wesley, 2002. ISBN 978-0321127426.
- BASS, Len; CLEMENTS, Paul; KAZMAN, Rick. Software Architecture in Practice. Addison-Wesley, 2012. ISBN 978-0321815736.
- CLEMENTS, Paul et al. Documenting Software Architectures: Views and Beyond. Addison-Wesley, 2010. ISBN 978-0321552686.
- ROZANSKI, Nick; WOODS, Eóin. Software Systems Architecture: Working With Stakeholders Using Viewpoints and Perspectives. Addison-Wesley, 2011. ISBN 978-0321718334.
- ALBIN, Stephen T. The Art of Software Architecture: Design Methods and Techniques. Wiley, 2003. ISBN 978-0471267734.


