# Padrões aplicados

Foram aplicados padrões de duas categorias:
- Gang of Four (GoF)
- Fowler's Patterns

A relação destes e as suas explanações seguem nas tabelas abaixo:

## GoFs

|      Tipo      |       Padrão      | Implementado por | Explanação                                                                                                                                                                                                                                                                                                                    |
|:--------------:|:-----------------:|:----------------:|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Criacional     | *Factory Method*  | *Django*  | A maneira com a qual o Django implementa a sua estrutura de forms faz uso de uma Factory de Fields, onde existe uma fábrica de inputs dado os atributos necessários para se construir um objeto. |
| Estrutural     |  *Decorator*      | Equipe/*Django*           | O decorator foi implementado em várias partes do código. Para requerer o login do usuário, utilizou-se um decorador já implementado pelo framework. Para se mostrar os logs das funções na saída padrão do sistema, implementou-se um decorador de debug. Por fim, implementou-se um decorador para inserir os atributos necessários para construir o esquema observador-observado em tempo de execução |
| Estrutural     | *Facade*          | *Django*         | O *Django* em sua estrutura já implementa o padrão *Facade*, o arquivo de *URL's* (gerado pelo *framework*) é onde é feito todo o gerenciamento de rotas da aplicação. Dentro do *Django* existem vários *apps* e cada um tem a sua *url*, o arquivo *urls.py* nada mais é do que uma fachada que gerencia outras fachadas. |
| Comportamental | *Template Method* | *Django*         | O *Template Method* é implementado em diversas partes do *framework*. O GitPub utiliza fortemente os templates de models fornecidos pelo pacote *Django.models*.
| Estrutural | *Observer* | Equipe         | A implementação do observer, apesar de não ter sido feita em sua forma purista (mas simulada), apresenta uma maneira "pytônica" de se implementar o padrão. Por meio de decoradores providos pelo pacote [Notifyr](https://github.com/victorcmoura/notifyr), é possível incluir os métodos do esquema observador-observado em tempo de execução em qualquer classe Python. A sua aplicação no GitPub possibilita o envio de emails aos matriculados na disciplina toda vez que um novo projeto for criado.
| Criacional | *Singleton* | Equipe         | Para o sistema de logs, foi implementado um Singleton que gerencia a impressão dos logs na saída padrão do sistema. Junto com decoradores, é possível exibir os logs de todas as funções implementadas no sistema. Os decoradores sempre tentam criar um objeto que escreve o resultado na saída padrão, entretanto, há apenas uma instância deste objeto, economizando recursos computacionais.

## Fowler's Patterns (Architectural Patterns)

Os padrões de Fowler foram descritos no livro *Patterns of Enterprise Application Architecture* em 2002 por Martin Fowler. Estes padrões definem esquemas arquiteturais observados em grandes *frameworks* hoje em dia, como Ruby on Rails e Python Django.

|       Padrão      | Implementado por | Explanação                                                                                                                                                                                                                                                                                                                    |
|:-----------------:|:----------------:|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| *Active Record*  | *Django*  | Este padrão define um encapsulamento da comunicação e interação com o banco de dados na camada de programação da aplicação, disponibilizando todo o domínio lógico para acesso ao dado. Este padrão é percebido no *Django.db*, módulo que encapsula toda a comunicação da aplicação com o banco de dados. |
| *Class Table Inheritance*  | *Django*  | Define-se que cada modelo de dados deve possuir uma tabela exclusiva no banco de dados. As *Django Models* utilizam fortemente deste esquema, inclusive em caso de herança entre models. |
| *Identity Field*  | *Django*  | Todo objeto da aplicação possui um ID que é a sua chave primária no banco de dados. Sua intenção é manter a identidade dos objetos persistidos. O módulo *Django.db* somado ao *Django.models* apresentam exatamente este comportamento para manter a identidade dos objetos criados. |
| *Template View*  | *Django*  | Este padrão arquitetural é identificado pela inserção de marcadores dentro do código HTML. Nas *Django Templates* é possível inserir marcadores para tornar o *render* do HTML algo dinâmico sem o uso de outra linguagem, como o JavaScript. |