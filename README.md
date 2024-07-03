
ATIVIDADE – Spring
Atividade prática – Desenvolvendo o Backend com Spring


Instruções gerais:
Utilize o Spring Tool Suite (STS) para desenvolver os projetos Spring.
Crie um repositório no Github para cada projeto Spring
Ao concluir uma nova etapa do projeto, envie todas as alterações para o Repositório do projeto criado na sua conta pessoal do Github (a pasta inteira)
Envie o link do repositório no Github através da Plataforma da Generation na data indicada
Caso seja solicitado, adicione os links individuais dos arquivos .JAVA indicados, no item: Adicione um dos links da sua entrega, localizada depois do link do Repositório, na tela de entrega da atividade na plataforma, para validação da atividade.
Validar: Postagem.java, PostagemRepository.java e PostagemController.java
Mantenha as entregas das Atividades em dia na Plataforma da Generation


EXERCÍCIOS

Boas práticas:

Crie o Repositório do projeto no Github.
Crie o projeto no Spring Initialzr, seguindo as boas práticas de projeto.
Configure o arquivo application.properties para criar e acessar o Banco de dados MySQL no seu computador.
Execute a sua aplicação no STS e verifique se o Banco de dados foi criado no MySQL Workbench.
Crie a Classe Model e coloque todos os atributos necessários, incluindo os Métodos Get e Set e as Anotações. Não é necessário criar um Método Construtor.
Execute a sua aplicação no STS e verifique se a tabela foi criada no MySQL Workbench.
Crie a Interface Repository.
Crie a Classe Controller.
Na Classe Controller, crie o Método getAll().
Insira dados na tabela através do MySQL Workbench.
Teste o método getAll() através do Insomnia.
Ao final desta atividade, inicialize a pasta do projeto como um repositório Git e faça a conexão com o repositório remoto no Github.
Envie o projeto para o repositório remoto.
Na entrega das atividades na Plataforma, efetue a validação das 2 Classes e da Interface desenvolvidas, utilizando as seguintes camadas:
Postagem: Camada model
PostagemRepository: Camada repository
PostagemController: Camada controller
Caso ainda fique alguma dúvida, consulte os instrutores da sua turma pelo Discord

 ATIVIDADE CRUD BACKEND BLOG-PESSOAL – PARTE 01

O Projeto Blog Pessoal possui as seguintes características:

O Banco de dados da aplicação será o db_blogpessoal.
Na Camada Model será criada a Classe Postagem com os seus respectivos atributos.
A Classe Postagem criará a Tabela tb_postagens no Banco de dados db_blogpessoal.
Na Camada Repository será criada a Interface PostagemRepository (com a capacidade de se comunicar com o banco de dados MySQL).
Na Camada de Controller será criada a Classe PostagemController. 
Na Camada Controller será criado um endpoint:
getAll() com a capacidade de listar todas as Postagens.
