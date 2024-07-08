ATIVIDADE CRUD BACKEND BLOG-PESSOAL – PARTE 03

Na terceira parte do Projeto Blog Pessoal iremos adicionar as seguintes características:

01 – Criar o Recurso Tema

Na Camada Model será criada a Classe Tema com os seus respectivos atributos.
A Classe Tema criará a Tabela tb_temas no Banco de dados db_blogpessoal.
Na Camada Repository será criada a Interface TemaRepository (com a capacidade de se comunicar com o banco de dados MySQL).
Na Interface TemaRepository vamos adicionar o Método de busca específica:
findAllByDescricaoContainingIgnoreCase() com a função de trazer todes os Temas cuja descrição possua a palavra pesquisada.
Na Camada Controller será criada a Classe TemaController. 
Na Classe TemaController serão criados os seguintes endpoints:
getAll() com a capacidade de listar todes os Temas.
getById() com a função de trazer um único Tema identificado pelo id.
getByDescricao() com a função de trazer todes os Temas cuja descrição possua a palavra pesquisada.
post() com a função de gravar (persistir) um novo Tema no Banco de dados.
put() com a função de atualizar os dados de um Tema.
delete() com a função de apagar um Tema no banco de dados.



02 – Criar o Relacionamento entre as Classes Tema e Postagem

Na Camada Model, na Classe Tema, crie a Relação OneToMany com a Classe Postagem. Não esqueça de adicionar todas as Anotações e Métodos Get e Set necessários.
Na Camada Model, na Classe Postagem, crie a Relação ManyToOne com a Classe Tema. Não esqueça de adicionar todas as Anotações e Métodos Get e Set necessários.
Em especial, não esqueça da anotação @JsonIgnoreProperties para inibir a Recursividade no relacionamento.
Faça os ajustes necessários no Insomnia para Inserir e Atualizar os dados do Recurso Postagem, habilitando o Relacionamento.
Teste todes os Métodos dos Recursos Tema e Postagem no Insomnia.
Verifique nos Testes se ao listar as Postagens, o respectivo Tema associado é exibido.

Verifique nos Testes se ao listar os Temas, as Postagens associadas serão exibidas.

