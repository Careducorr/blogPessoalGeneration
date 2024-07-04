ATIVIDADE CRUD BACKEND BLOG-PESSOAL – PARTE 02

Na segunda parte do Projeto Blog Pessoal iremos adicionar as seguintes características:

Na Interface PostagemRepository vamos adicionar o Método de busca específica:
findAllByTituloContainingIgnoreCase() com a função de trazer todas as  Postagens cujo título possua a palavra pesquisada.
Na Classe PostagemController vamos adicionar os seguintes Métodos:
getById() com a função de trazer uma única Postagem identificada pelo id.
getByTitulo() com a função de trazer todas Postagens cujo titulo possua a palavra pesquisada.
post() com a função de gravar (persistir) uma nova Postagem no banco de dados.
put() com a função de atualizar os dados de uma Postagem.
delete() com a função de apagar uma Postagem no banco de dados.
