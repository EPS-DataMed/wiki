<br/>

<div style="display: flex; flex-direction: column; justify-content: center; align-items:center;">
    <img src="https://dansousamelo.github.io/RQ_ISP/assets/backlog/BACKLOG-ICON.png" width="200" height="200" style="filter: brightness(0%);"ss />
</div>

<br/>

Neste documento, estão delineadas políticas de contribuições do repositório do projeto DataMed e tem como objetivo explicar os procedimentos a serem realizados para se contribuir com o projeto. Esse documento foi adaptado da [Políticas do Repositório do Projeto College Flow](https://fga-eps-mds.github.io/CollegeFlow/#/policies).

## Histórico de versões

| Versão |    Data    |     Descrição     |                      Autor(es)                       | Revisor(es) |
| :----: | :--------: | :---------------: | :--------------------------------------------------: | :---------: |
| `1.0`  | 16/04/2024 | Criando documento | [Grupo 01](/grupos/grupo_01?id=integrantes-do-grupo) |      -      |


Aqui se encontram:

- Política de Issue
- Política de Branch
- Política de Commit
- Política de Pull Request

## Nomenclaturas gerais:

A Tabela 1 a seguir representa as nomenclaturas gerais que serão utilizadas para atribuir contexto as Issues, Branchs, Commits e Pull Requests

| Nomenclatura | Descrição                                                                                     |
| ------------ | --------------------------------------------------------------------------------------------- |
| feat         | Representa adicão de novos elementos ao projeto.                                              |
| refac        | Indica modificão de elementos já presentes no projeto para melhorar performance, design, etc. |
| fix          | Indica o conserto de problemas/erros existentes no projeto.                                   |
| docs         | Indica modificação na documentação do projeto                                                 |

<div style="text-align: center">
<p> Tabela 1: Nomenclaturas (Fonte: autor, 2024). </p>
</div>

## Políticas de Issue

- Antes de criar uma Issue certifique-se se já não existe uma relacionada ao problema ou situação utilizando a ferramenta de busca de Issues.
- Ao criar uma Issue o no GitLab do projeto adicione uma nomenclatura, de acordo com a Tabela 1, em letras maiúsculas em seguida da descrição do problema.
> **Exemplo**: Criação de uma nova feature para adição de imagens. <code>[FEAT]: Add images</code>
- A seguir na descrição, adicione uma descrição apoiada de critérios de aprovação
- Se certifique de se assinalar a pessoa responsável pela Issue
- Adicione as Labels e Milestones aplicaveis

## Políticas de Branch

Branchs devem seguir as seguintes regras.

- Branch **master** representa uma versão estável do produto, contendo código testado e versionado. Essa branch parte da branch **develop** através de pull requests aprovados no fim de cada release

  Regras:

  1. Existe apenas uma branch **master**.
  2. Não são permitidos commits feitos diretamente na master.

- Branch **develop** contém a versão mais atualizada do código que está sendo desenvolvido. Essa branch está sempre sincronizada com a **master** e é base para as branches **feat**.

  Regras:

  1. Existe apenas uma branch **develop**.

### Nomenclatura de branches

Ao criar novas branches iremos dividí-las em uma das 4 categorias representadas na Tabela 1. Esses serão prefixos utilizados para criação da branch.

> **Exemplo**: Criação de uma nova feature para adição de imagens. <code>feat/add_images</code>

## Políticas de Commits

Commits devem ser escritos de forma clara e breve, em inglês, descrevendo as alterações feitas.

Regras para escrita das mensagens no commits:

1. Utilizar prefixos pré-estabelecidos na Tabela 1.
2. Faça commits **pequenos**, não agrupe múltiplas funcionalidades em um commmit! Divida nos menore blocos de código possível.
3. Em caso de commit realizado por mais de uma pessoa, utilize o **coauthor** para dar créditos.

> **Exemplo**: Adição de imagens a página web. <code>feat: add images</code>

## Políticas de Pull Request

Pull Requests devem conter no título abordar a issue trabalhada. Na descrição é importante prover todos os links necessários para termos um entendimento completo da task em questão.
Estrutura básico para o nome do Pull request: <code>[#IssueCode/Prefix]: Problema principal</code>

> **Exemplo**: <code>[#53/FEAT]: Crud to Admin</code>

Regras

1. Linkar quem participou do Pull request.
2. Ter dois approves antes de dar mergear o Pull request.
3. Ter aprovação nos testes.
4. Linkar PR com a issue(es) relacionada(as).

Observações

1. PRs devem ser pequenos para ter uma revisão de boa qualidade.
2. Use stack de PRs.
3. Evite PRs com múltiplas lógicas que podem ser separadas.

## Referências

* <article> College Flow. Github.io. Disponível em: https://fga-eps-mds.github.io/CollegeFlow/#/policies. Acesso em: 17 abr. 2024.</article>

* <article> Padrões e nomenclaturas no Git. Brunodulcetti.com. Disponível em: https://www.brunodulcetti.com/padroes-e-nomenclaturas-no-git/. Acesso em: 17 abr. 2024.</article>

* <article> Writing Git commit messages. Tumblr. Disponível em: https://365git.tumblr.com/post/3308646748/writing-git-commit-messages. Acesso em: 17 abr. 2024.</article>

* <article> SIMOHAMED MARHRAOUI. Using stacked pull requests in GitHub - LogRocket Blog. LogRocket Blog. Disponível em: https://blog.logrocket.com/using-stacked-pull-requests-in-github/. Acesso em: 17 abr. 2024.</article>

* <article> Acácia. Github.io. Disponível em: https://fga-eps-mds.github.io/2019.2-Acacia/#/policies?id=pol%c3%adtica-de-migra%c3%a7%c3%b5es. Acesso em: 17 abr. 2024.</article>

* <article> FACHAL, Manuel. Git-flow Applied to a Real Project - Empathy.co - Medium. Medium. Disponível em: https://medium.com/empathyco/git-flow-applied-to-a-real-project-c08037e28f88. Acesso em: 17 abr. 2024.</article>