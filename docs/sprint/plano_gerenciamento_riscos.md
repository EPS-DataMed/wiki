<br/>

<div style="display: flex; flex-direction: column; justify-content: center; align-items:center;">
    <img src="https://dansousamelo.github.io/RQ_ISP/assets/backlog/BACKLOG-ICON.png" width="200" height="200" style="filter: brightness(0%);" />
</div>

<br/>

Neste documento, estão delineadas o plano de risco do projeto. Este plano aborda de maneira detalhada as potenciais ameaças que podem impactar o andamento das atividades, bem como as estratégias propostas para mitigação desses riscos. A identificação e análise de riscos foram realizadas através de uma combinação de técnicas qualitativas e quantitativas, garantindo uma visão abrangente e precisa dos possíveis obstáculos. Além disso, são descritas as responsabilidades dos membros da equipe em relação à gestão de riscos, incluindo a implementação de ações preventivas e corretivas.

## Histórico de versões

Esta seção apresenta o histórico de versões do documento, detalhando as mudanças realizadas e os responsáveis por cada alteração.

| Versão |    Data    |              Descrição               |                      Autor(es)                       | Revisor(es) |
| :----: | :--------: | :----------------------------------: | :--------------------------------------------------: | :---------: |
| `1.0`  | 16/04/2024 | Criando documento de Plano de Risco | Vitor Diniz |      -      |

## Introdução

O planejamento de riscos é uma das etapas fundamentais no processo de planejamento de um projeto, pois ao identificar os possíveis riscos, torna-se viável estabelecer estratégias para mitigar os impactos que esses riscos possam ter sobre o projeto. Os riscos de um projeto podem comprometer o seu planejamento, cronograma e custo, podendo estar relacionados a diversos fatores, como custo, tempo, pessoas, recursos, clientes, requisitos, entre outros <a href=./#referencias>¹</a>. Com o objetivo de identificar, analisar e monitorar esses riscos, foi elaborado este plano de gerenciamento de riscos.

### Tipos de risco

Para a classificação dos riscos, foram consideradas as seguintes categorias:

- Externo
- Gerencial
- Organizacional
- Técnico

## Definições

### Probabilidade e impacto dos riscos

A tabela a seguir define os níveis de probabilidade e impacto dos riscos, proporcionando uma base para a avaliação dos riscos identificados.

| Nível | Probabilidade | Porcentagem de certeza |
| :---: | :---: | :---: |
| 1 | Muito baixa | 0% - 19% |
| 2 | Baixa | 20% - 39% |
| 3 | Média | 40% - 59% |
| 4 | Alta | 60% - 79% |
| 5 | Muito alta | 80% - 100% |

### Impacto

A tabela a seguir descreve os níveis de impacto dos riscos, auxiliando na determinação da gravidade de cada risco identificado.

| Nível | Impacto |
| :---: | :---: |
| 1 | Muito baixo |
| 2 | Baixo |
| 3 | Médio |
| 4 | Alto |
| 5 | Muito alto |

### Matriz de probablidade X impacto

A matriz de probabilidade e impacto combina as informações das tabelas anteriores para fornecer uma avaliação detalhada dos riscos.

| Probabilidade / Impacto | Muito baixo | Baixo | Médio | Alto | Muito alto |
| :---: | :---: | :---: | :---: | :---: | :---: |
| Muito baixa | 1 | 2 | 3 | 4 | 5 |
| Baixa | 2 | 4 | 6 | 8 | 10 |
| Média | 3 | 6 | 9 | 12 | 15 |
| Alta | 4 | 8 | 12 | 16 | 20 |
| Muito alta | 5 | 10 | 15 | 20 | 25 |

### Graus de risco

Os graus de risco são determinados pela matriz de probabilidade e impacto, conforme mostrado na tabela a seguir.

| Grau | Risco |
| :---: | :---: |
| 1 - 5 | Baixo |
| 6 - 12 | Médio |
| 15 - 25 | Elevado |

## Levantamento de riscos

### Tabela de Riscos

A tabela a seguir lista os riscos identificados para o projeto, junto com suas descrições e categorias correspondentes.

| Risco | Descrição                                         | Categoria      |
|-------|---------------------------------------------------|----------------|
| R01   | Desafios com as tecnologias selecionadas          | Técnico        |
| R02   | Desligamento de algum membro do projeto           | Gerencial      |
| R03   | Baixo envolvimento de algum integrante            | Gerencial      |
| R04   | Pouca integração entre os membros da equipe       | Gerencial      |
| R05   | Demora na liberação de documentação ou funcionalidades | Gerencial |
| R06   | Conflito de horários entre os integrantes         | Organizacional |
| R07   | Falha nas plataformas de comunicação              | Externo        |
| R08   | Problemas na definição da arquitetura             | Técnico        |
| R09   | Modificações no escopo do projeto                 | Gerencial      |
| R10   | Problemas de saúde de um integrante              | Externo        |
| R11   | Não disponibilidade do cliente                    | Externo        |
| R12   | Qualidade insuficiente do código fonte            | Técnico        |
| R13   | Falta de entrega de versões para testes do cliente | Gerencial     |
| R14   | Desatenção nas reuniões                           | Gerencial      |
| R15   | Sobrecarga de trabalho em um membro da equipe     | Gerencial      |
| R16   | Falha de equipamento                              | Externo        |
| R17   | Interdependência entre atividades                 | Organizacional |

### Causas e Consequências dos Riscos

A tabela a seguir detalha as causas e consequências de cada risco identificado, permitindo uma compreensão aprofundada de cada risco.

| Risco | Causa                                             | Consequência |
|-------|---------------------------------------------------|--------------|
| R01   | Inexperiência com as tecnologias utilizadas       | Baixa qualidade do produto e atrasos nas entregas |
| R02   | Questões pessoais e excesso de carga de trabalho  | Redução da capacidade de entrega da equipe |
| R03   | Motivação reduzida do integrante                  | Acúmulo de atividades não realizadas |
| R04   | Falta de compromisso e comunicação insuficiente entre os integrantes | Desalinhamento dentro da equipe |
| R05   | Planejamento inadequado e estimativas erradas     | Alterações no cronograma e descontentamento do cliente |
| R06   | Outras obrigações acadêmicas e pessoais           | Dificuldades de integração e participação limitada nas reuniões |
| R07   | Interrupções nos serviços de comunicação          | Delays na decisão |
| R08   | Requisitos mal levantados                         | Revisões frequentes e baixa qualidade do produto |
| R09   | Mudanças nos requisitos                           | Extensão de prazos e aumento de custos, levando à insatisfação do cliente |
| R10   | Problemas de saúde                                | Maior carga de trabalho para os demais membros |
| R11   | Falta de comprometimento e conflitos de agenda do cliente | Retrabalho e dificuldades em obter validações |
| R12   | Ausência de revisões adequadas e falta de expertise técnico | Crescimento no número de bugs e manutenção problemática |
| R13   | Falhas no processo de disponibilização para testes do cliente | Risco de erros na implementação e desagrado do cliente |
| R14   | Reuniões prolongadas                              | Produtividade reduzida durante os encontros |
| R15   | Distribuição desigual de tarefas                  | Concentração de conhecimento técnico em poucos indivíduos |
| R16   | Uso contínuo sem manutenção adequada              | Custos adicionais e atrasos nos projetos |
| R17   | Falta de sincronia nas atividades                 | Obstrução no avanço de outras tarefas |

### Prevenção e Ações para os Riscos

A tabela a seguir apresenta as medidas de prevenção e as ações propostas para cada risco identificado.

| Risco | Prevenção                                         | Ação |
|-------|---------------------------------------------------|------|
| R01   | Implementação de treinamentos                     | Prática de programação em dupla para disseminação de conhecimento |
| R02   | Incentivo constante e organização de horários     | Reajuste na alocação e planejamento de tarefas |
| R03   | Estímulo contínuo para envolvimento dos integrantes| Diálogo para entender e solucionar as dificuldades do integrante |
| R04   | Engajamento ativo em todas as reuniões            | Reagendamento de encontros para melhor conveniência |
| R05   | Estimativas realistas e planejamento detalhado    | Revisão das tarefas e prazos estabelecidos |
| R06   | Criação de um cronograma flexível                 | Formação de duplas para execução das tarefas |
| R07   | -                                                 | Uso de alternativas previamente estabelecidas para comunicação |
| R08   | Alinhamento com as necessidades e escopo do projeto| Revisão da arquitetura e das tecnologias adotadas |
| R09   | Definição clara e objetiva do escopo              | Atualização dos requisitos e escopo conforme as mudanças |
| R10   | Adoção de práticas de saúde recomendadas          | Redistribuição das responsabilidades |
| R11   | Acordo prévio sobre horários de reuniões com o cliente | Pedido de reagendamento de encontros com o cliente |
| R12   | Implementação de uma cobertura de testes completa e uso de ferramentas de análise de código | Identificação e refatoração dos componentes que comprometem a qualidade |
| R13   | Preparação antecipada do ambiente de testes       | Revisão e melhoria do processo de liberação para testes |
| R14   | Definição de agenda e limite de tempo para reuniões| Realização de encontros presenciais ocasionalmente |
| R15   | Equilíbrio na distribuição de tarefas             | Revisão e realocação das responsabilidades |
| R16   | Manutenção periódica dos equipamentos             | Reparo ou substituição dos equipamentos conforme necessário |
| R17   | Planejamento adequado das prioridades do projeto  | Revisão das prioridades e ajustes necessários |


## Referências

* <div> ESCRITÓRIO de Projetos. Objetivo do Plano de gerenciamento dos riscos. Disponível em: https://escritoriodeprojetos.com.br/downloads/send/8-modelos/129-plano-de-gerenciamento-dos-riscos. Acesso em: 30 abr. 2024.</div>

* <div>ISOTANI, Seiji; ROCHA, Rafaela. Gestão de Riscos em Projetos de Software. Disponível em: https://edisciplinas.usp.br/pluginfile.php/3385127/mod_resource/content/1/Aula10-GerenciaProjeto-Riscos.pdf. Acesso em: 30 abr. 2024.</div>
