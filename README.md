ATIVIDADE SECURITY BACKEND BLOG-PESSOAL

Nesta etapa, vamos implementar a segurança no Projeto Blog Pessoal:

Insira as Dependências: 
Spring Security
jjwt-api
jjwt-impl
jjwt-jackson
Na Camada Model será criada as Classes Usuario e UsuarioLogin com os seus respectivos atributos. 
A Classe UsuarioLogin não irá gerar tabela, logo não precisa de Anotações.
A Classe Usuario criará a Tabela tb_usuarios no Banco de dados db_blogpessoal.
Na Camada Repository será criada a Interface UsuarioRepository (com a capacidade de se comunicar com o banco de dados MySQL).
Na Interface UsuarioRepository vamos adicionar o Método de busca específica:
findByUsuario() com a função de trazer um usuário específico pelo e-mail (conteúdo do atributo usuário, da Model Usuario).
Na Camada Security serão criadas as Classes:
BasicSecurityConfig
UserDetailsImpl
UserDetailsServiceImpl
JwtService
JwtAuthFilter
Na Camada Service será criada a Classe UsuarioService
Implemente na Classe UsuarioService os Métodos:
cadastrarUsuario()
atualizarUsuario()
autenticarUsuario()
Na Camada Controller será criada a Classe UsuarioController. 
Na Classe UsuarioController serão criados os seguintes métodos:
getAll() com a capacidade de listar todos os Usuários.
getById() com a função de trazer um único Usuário identificada pelo id.
post() com a função de gravar (persistir) um novo Usuário no banco de dados.
put() com a função de atualizar os dados de um Usuário.
logar() com a função de efetuar login na API.
