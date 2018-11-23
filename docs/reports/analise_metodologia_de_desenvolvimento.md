### Histórico de Revisões

| Data       | Versão | Descrição            |         Autor             |
|:----------:|:------:|:--------------------:|:-------------------------:|
| 22/11/2018 | 1.0 | Criação do Documento  | [Victor Moura](https://github.com/victorcmoura) |


# Análise Crítica da Metodologia

# A metodologia

Durante a etapa de documentação, houve esforço para preparar a metodologia de desenvolvimento da aplicação GitPub. Foram feitos os seguintes artefatos:

- Folha de estilo
    - Baseada nas especificações PEP8, definiu uma maneira "Pytônica" de se escrever o código.
- Política de branches
    - Definiu uma maneira organizada de se nomear as branches do projeto.
- Política de commits
    - Definiu uma maneira organizada de se nomear os commits do projeto.
- Template de issue
    - Apresenta, ao usuário que vai criar a issue, um template que define o formato de texto que a issue deve apresentar.
- Template de Pull Request
    - Apresenta, ao usuário que vai criar o pull request, um template que define o formato de texto que o PR deve apresentar.

Além disso, foi definido que utilizaríamos a metodologia Scrum para guiar o nosso processo de desenvolvimento. A organização era feita da seguinte maneira:

- Sprints de 7 dias iniciando na segunda-feira
- Revisão/Retrospectiva/Planejamento de sprint todo domingo de 21h30 às 22h30, via hangouts
- Daily meeting remota de segunda a quinta-feira, 21h30 às 22h30

Os artefatos resultantes definidos foram:

- Backlog do produto
- Backlog da sprint documentado na plataforma ZenHub
- Incrementos feitos em código

# Transparência no desenvolvimento

Como iniciativa para melhor documentar as dailies, foi decidido que elas seriam feitas na plataforma GitHub, por meio de issues abertas durante o horário definido previamente. Logo, percebemos que seria trabalhoso demais abrir uma issue todos os dias para documentar o que estava sendo feito. Como tentativa de remover responsabilidades dos membros do time para executar tal tarefa, foi criado um bot que, utilizando a conta do GitHub do LAPPIS (conta disponível para os membros do laboratório realizarem automações de ambiente), abria e fechava as issues automaticamente sempre no horário definido:

![Exemplo de issue daily](https://github.com/Desenho2018-2-GitPub/docs/blob/master/docs/images/daily_automatica.png?raw=true)

A experiência foi, inicialmente, positiva e possibilitou apresentar maior transparência sobre o nosso processo de desenvolvimento:

![Exemplo de issue daily](https://github.com/Desenho2018-2-GitPub/docs/blob/master/docs/images/daily_automatica2.png?raw=true)

O repositório contendo o código necessário para rodar tal script está disponível [no repositório na organização](https://github.com/Desenho2018-2-GitPub/CronDailyMeeting) e funciona a partir de um cronjob executado em um container Docker hospedado em uma máquina virtual no Amazon Elastic Compute Cloud (Amazon EC2).

Além das dailies, definiu-se que todo o projeto teria suas tarefas documentadas em formato de issues no GitHub e seriam organizadas de acordo com a funcionalidade de seleção de *milestones* disponibilizada pela plataforma. As issues deveriam conter as tarefas necessárias para o desenvolvimento, eventuais problemas e quaisquer comunicações gerais relacionadas ao projeto. As discussões sobre as issues ficariam reservadas para o campo de comentários, onde seria o espaço ideal para se atualizar os demais membros do andamento da tarefa.

# Influência da disciplina no projeto

Definidas as ferramentas de trabalho, começou-se o desenvolvimento a partir da modelagem feita inicialmente. Boa parte da equipe ainda não possuía os conhecimentos necessários para se desenvolver e, não atentos a isto, não foi feito um plano de distribuição de conhecimento. Tal fato reduziu a cadência de contribuições e, dado o ritmo da disciplina, a situação passou a ser crítica, apresentando cenário no qual a metodologia era completamente negligenciada. Após o período no qual estávamos concentrando os nossos esforços pessoais para a avaliação escrita da disciplina, valendo 70% da nota final, voltou-se a pensar no projeto.

Até então, havia uma aplicação com toda a gerência de configuração de ambiente feita, com o banco de dados modelado mas sem nenhuma funcionalidade disponível para o usuário final. Observou-se que, com o aproximar da última dinâmica, o ritmo de desenvolvimento acelerou-se de forma intensa para que houvesse a entrega do produto esperado. Com o fim da implementação das funcionalidades *core*, houve curiosidade para entender qual havia sido o problema que ocasionou tal situação. Iniciou-se então, um levantamento entre alguns membros da disciplina, que faziam parte de projetos diferentes, para avaliar se o mesmo havia ocorrido em outros times.

Conversas informais apontavam que a desordem era generalizada entre as equipes e, portanto, poderia estar relacionado a algum fator em comum. Métricas foram coletadas com foco na análise da hipótese de que os times diminuíram o ritmo de trabalho e o interesse pessoal no projeto dada a importância dada ao período da avaliação escrita. Os resultados obtidos seguem abaixo:

## Contribuições (commits)

Em relação aos commits, observou-se que, em um determinado período de setembro a outubro, as equipes apresentaram poucas ou nenhuma contribuição. Além disso, percebe-se que o ritmo de trabalho tende a aumentar significativamente quando a data da entrega se aproxima. Sabemos que tal prática geralmente vem acompanhada de negligências em relação às políticas de desenvolvimento, diminuindo a qualidade geral da organização e do resultado final de cada time. Os exemplos seguem abaixo:

### Exemplo 1
![exemplo1](https://github.com/Desenho2018-2-GitPub/docs/blob/master/docs/images/analise_critica_metodologia/Commits/1/docs.png?raw=true)

### Exemplo 2
![exemplo2](https://github.com/Desenho2018-2-GitPub/docs/blob/master/docs/images/analise_critica_metodologia/Commits/2/2.png?raw=true)

### Exemplo 3
![exemplo3](https://github.com/Desenho2018-2-GitPub/docs/blob/master/docs/images/analise_critica_metodologia/Commits/3/code.png?raw=true)

### Exemplo 4
![exemplo4](https://github.com/Desenho2018-2-GitPub/docs/blob/master/docs/images/analise_critica_metodologia/Commits/5/Captura%20de%20tela%20de%202018-11-21%2009-39-30.png?raw=true)

### Engajamento dos membros

Para avaliar o engajamento dos membros de cada time, optou-se por coletar métricas relacionadas às issues no GitHub. Entende-se que membros engajados costumam abrir mais issues e comentar nelas com mais frequência. Os resultados de cada uma delas está apresentado abaixo.

#### Issues abertas por semana

##### Exemplo 1

![exemplo1](https://github.com/Desenho2018-2-GitPub/docs/blob/master/docs/images/analise_critica_metodologia/Issues%20abertas%20por%20semana/1.png?raw=true)

##### Exemplo 2

![exemplo1](https://github.com/Desenho2018-2-GitPub/docs/blob/master/docs/images/analise_critica_metodologia/Issues%20abertas%20por%20semana/2.png?raw=true)

##### Exemplo 3

![exemplo1](https://github.com/Desenho2018-2-GitPub/docs/blob/master/docs/images/analise_critica_metodologia/Issues%20abertas%20por%20semana/3.png?raw=true)

##### Exemplo 4

![exemplo1](https://github.com/Desenho2018-2-GitPub/docs/blob/master/docs/images/analise_critica_metodologia/Issues%20abertas%20por%20semana/gitpub.png?raw=true)

Com uma exceção, é possível observar que, mesmo havendo diferenças entre os times, houve a tendência da redução de issues abertas justamente na sprint na qual a queda de contribuições foi menor.

#### Caracteres comentados por semana

##### Exemplo 1

![exemplo1](https://github.com/Desenho2018-2-GitPub/docs/blob/master/docs/images/analise_critica_metodologia/Total%20de%20caracteres%20comentados%20por%20semana/1.png?raw=true)

##### Exemplo 2

![exemplo1](https://github.com/Desenho2018-2-GitPub/docs/blob/master/docs/images/analise_critica_metodologia/Total%20de%20caracteres%20comentados%20por%20semana/2.png?raw=true)

##### Exemplo 3

![exemplo1](https://github.com/Desenho2018-2-GitPub/docs/blob/master/docs/images/analise_critica_metodologia/Total%20de%20caracteres%20comentados%20por%20semana/gitpub.png?raw=true)

Apesar de um dos times não ter trabalhado com comentários nas issues, por isso esta métrica apresenta um exemplo a menos, também é possível observar que a queda de engajamento é visível durante o período analisado. No último caso, ainda percebe-se que o costume de não comentar nas issues foi levado adiante mesmo com a retomada das contribuições.

# Conclusão

Dadas as métricas analisadas e a hipótese inicialmente levantada, acredita-se que a avaliação escrita (feita no dia 19/10/2018) e os dias que a antecederam influenciaram diretamente na queda de produtividade dos projetos e, consequentemente, na aplicação correta das metodologias definidas. Sugere-se que o método de avaliação da disciplina seja reavaliado para que este problema não ocorra novamente nos próximos semestres. Este documento apresenta a opinião da equipe.
