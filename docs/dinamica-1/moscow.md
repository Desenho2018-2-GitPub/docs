### Histórico
|Data|Versão|Descrição|Autor(es)|
|--|--|--|--|
| 01/09/2018 | 0.1 | Criação modelo da tabela do MoSCoW e adicionando primeiras funcionalidades | Kamilla Costa |
| 03/09/2018 | 1.1 | Revisão de conteúdo  | [Romeu Antunes](https://github.com/RomeuCarvalhoAntunes) |


1. [Introdução](#1-introdução)  
1.1. [Propósito](#11-propósito)  
1.2. [Escopo](#12-escopo)  
2. [Objetivos](#2-objetivos)  
3. [MoScoW](#4-moscow)  

## 1. Introdução
### 1.1. Propósito
<p align="justify">&emsp;&emsp;O documento presente tem a finalidade de apresentar e estabelecer uma visão ampla sobre priorização de requisitos por meio da técnica 'MoSCoW' realizada em cima das funcionalidades identificadas no sistema GitPub.</p>

### 1.2. Escopo
<p align="justify">&emsp;&emsp;Será apresentada aqui a análise de priorização feita em cima das funcionalidades identificadas dentro do sistema GitPub. As marcações de <i>"must"</i>, <i>"should"</i>, <i>"could"</i> e <i>"would"</i>, indicadas pela técnica de priorização, serão utilizadas com a finalidade de  priorizar tais funcionalidades.</p>

## 2. Objetivos
<p align="justify">&emsp;&emsp;Com a realização da técnica de priorização 'MoSCoW', pretende-se identificar e estabelecer funcionalidades mais necessárias no sistema, aquelas que possuem maior valor do ponto do vista do usuário e também aquelas que são básicas do ponto de vista dos desenvolvedores.</p>

## 3. MoSCoW

### Requisitos Funcionais
| *Label* | Nome | Priorização |
| ------- | ---- | ----------- |
| RF-01 | O sistema deve permitir o cadastro de usuários | Must have OK|
| RF-02 | O sistema deve permitir a visualização dos projetos contidos em uma disciplina | Must have OK|
| RF-03 | O sistema deve permitir buscar os conteúdos por meio de filtros | Could have |
| RF-04 | O sistema deve permitir comentários nos projetos | Should have OK|
| RF-05 | O sistema deve permitir o usuário linkar arquivos do Git com um projeto | Must have |
| RF-06 | O sistema deve permitir o usuário linkar arquivos, via upload, com um projeto | Should have |
| RF-07 | O sistema deve permitir o gerenciamento de disciplinas | Must have OK|
| RF-08 | O sistema deve permitir o gerenciamento de projetos | Must have OK|
| RF-09 | O sistema deve permitir o gerenciamento de comentários | Must have |

### Requisitos Não Funcionais
| *Label* | Nome | Priorização |
| ------- | ---- | ----------- |
| RNF-01 | O sistema deve possuir boa usabilidade | Should have OK|
| RNF-02 | O sistema deve apresentar bom desempenho | Should have |
| RNF-03 | O sistema deve possuir bom controle de permissões | Must have |
| RNF-04 | O sistema deve ser confiável | Should have OK|

#### Interações
|ID|Descrição|Must|Should|Could|Would||
|--|--|--|--|--|--|--|
|1|Cadastrar usuário|x|||| OK
|2|Fazer login do usuário|x||||OK
|3|Visualizar disciplina|x||||OK
|4|Visualizar semestre|x||||OK
|5|Visualizar projeto|x||||OK
|7|Comentar||x|||OK
|8|Visualizar projetos para usuários logados|x||||
|9|Matricular em disciplina|x||||OK
|10|Registrar projeto|x||||OK
|11|Criar disciplina|x||||OK
|12|Remover aluno da disciplina||x|||
|13|Gerenciar disciplina|x||||OK
|14|Mudar roles de usuário||x|||
|15|Fazer upload de arquivo|x||||
|16|Fazer integração de arquivos do github e gitlab|x||||
|17|Criar label|||x||
|18|Pesquisar label|||x||
|19|Priorização de disciplinas no frontend||||x|
|20|Seguir usuário|||x||
|21|Curtir projeto|||x||
|22|Curtir comentário||||x|
|23|Responder comentário|||x||
|24|Bloquear comentários ofensivos|x||||
|25|Deixar de seguir usuário|||x||
|26|Editar perfil|||x||OK
|27|Alterar senha|||x||
|28|Alterar foto||||x|
|29|Alterar nome|||x||OK
|30|Alterar email||||x|OK
|31|Alterar biografia||x|||OK
|32|Notificação de registro de novo projeto||||x|
|33|Pesquisar usuário||||x|
|34|Marcar, como favorito, determinado projeto||||x|
|35|Visualizar atividades recentes do usuário||||x|
|36|Editar idioma||||x|
|37|Sair da conta de usuário|x||||OK
|38|Visualizar projetos em que o usuário foi adicionado||||x|OK
|39|Desvinculo Usuário/Disciplina||x|||OK
|40|Vínculo Projeto/Disciplina|x||||OK
|41|Forúm de dúvidas||||x|
