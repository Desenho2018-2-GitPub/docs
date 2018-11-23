### Histórico de Revisões

| Data       | Versão | Descrição            |         Autor             |
|:----------:|:------:|:--------------------:|:-------------------------:|
| 22/11/2018 | 1.0 | Criação do Documento  | [Victor Moura](https://github.com/victorcmoura) |


# Análise Crítica da Metodologia de Desenvolvimento

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

Como iniciativa para melhor documentar as dailies, foi decidido que elas seriam feitas na plataforma GitHub, por meio de issues abertas durante o horário definido previamente. Logo, percebemos que seria trabalhoso demais abrir uma issue todos os dias para documentar o que estava sendo feito. Como tentativa de remover responsabilidades dos membros do time para executar tal tarefa, foi criado um bot que, utilizando a conta do GitHub do LAPPIS (conta disponível para os membros do laboratório realizarem automações de ambiente), abria e fechava as issues automaticamente sempre no horário definido:

![Exemplo de issue daily](https://github.com/Desenho2018-2-GitPub/docs/blob/master/docs/images/daily_automatica.png?raw=true)

A experiência foi, inicialmente, positiva e possibilitou apresentar maior transparência sobre o nosso processo de desenvolvimento:

![Exemplo de issue daily](https://github.com/Desenho2018-2-GitPub/docs/blob/master/docs/images/daily_automatica2.png?raw=true)

O repositório contendo o código necessário para rodar tal script está disponível [no repositório na organização](https://github.com/Desenho2018-2-GitPub/CronDailyMeeting) e funciona a partir de um cronjob executado em um container Docker hospedado em uma máquina virtual no Amazon Elastic Compute Cloud (Amazon EC2).

Definidas as ferramentas de trabalho, iniciou-se o desenvolvimento a partir da modelagem feita inicialmente. Boa parte da equipe ainda não possuía os conhecimentos necessários para se desenvolver e, não atentos a isto, não foi feito um plano de distribuição de conhecimento. Tal fato reduziu a cadência de contribuições e, dado o ritmo da disciplina, a situação passou a ser crítica, apresentando cenário no qual a metodologia era completamente negligenciada. Após o período no qual estávamos concentrando os nossos esforços pessoais para a avaliação escrita da disciplina, valendo 70% da nota final, voltou-se a pensar no projeto.

Até então, havia uma aplicação com toda a gerência de configuração de ambiente feita, com o banco de dados modelado mas sem nenhuma funcionalidade disponível para o usuário final. Observou-se que, com o aproximar das dinâmicas, o ritmo de desenvolvimento acelerou-se de forma intensa para que houvesse a entrega do produto esperado. Com o fim da implementação das funcionalidades *core*, houve curiosidade para entender qual havia sido o problema que ocasionou tal situação. Iniciou-se então, um levantamento entre alguns membros da disciplina, que faziam parte de projetos diferentes, para avaliar se o mesmo havia ocorrido em outros times.

Conversas informais apontavam que a desordem era generalizada entre as equipes e, portanto, poderia estar relacionado a algum fator em comum. Métricas foram coletadas com foco na análise da hipótese de que os times diminuíram o ritmo de trabalho e o interesse pessoal no projeto dada a importância dada ao período da avaliação escrita. Os resultados obtidos seguem abaixo:

#todo