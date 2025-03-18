🚀 Projeto: Sistema de Cadastro de Usuários e Pets
Este projeto faz parte de uma atividade prática para o curso técnico em informática do Colégio ULBRA São Lucas. Desenvolvido por Bruno Martinho.

📋 Introdução Técnica
Este sistema utiliza as seguintes tecnologias e conceitos:

Java: Linguagem de programação principal
MySQL: Sistema de gerenciamento de banco de dados
POO: Programação Orientada a Objetos
DAO: Data Access Object (padrão para persistência de dados)
Swing: Framework para interfaces gráficas
🎯 Objetivo
Criar um sistema de cadastro simples para praticar manipulação de banco de dados, POO e interfaces gráficas.
Implementar um sistema de login e validação de senha forte.
Criar e manipular objetos utilizando boas práticas de programação.
🖥️ Pré-requisitos
Java JDK 8 ou superior
MySQL 5.7 ou superior
NetBeans IDE 8.2 ou superior
XAMPP (para gerenciamento do MySQL)
Conhecimentos básicos em Java e SQL
📂 Estrutura de Pastas
src/main/java/com/seuprojeto/
├── br.ulbra.entity/
│   ├── Usuario.java
│   ├── Pet.java
├── br.ulbra.dao/
│   ├── UsuarioDAO.java
│   ├── PetDAO.java
│   ├── ConnectionFactory.java
├── br.ulbra.view/
│   ├── FrmLogin.java
│   ├── FrmPrincipal.java
│   ├── FrmCadUsuario.java
│   ├── FrmCadPet.java
🔣 Legenda
✅ Requisito obrigatório - Deve ser implementado
🧑💻 Usuário - Relacionado ao cadastro e gerenciamento de usuários
🐶 Pet - Relacionado ao cadastro e gerenciamento de pets
🏢 Banco de Dados - Relacionado à configuração e manipulação do banco de dados
🏢 Banco de Dados
📐 Diagrama Entidade Relacionamento (DER)

🧪 Requisitos (Divididos por Ação)
🧑💻 Usuário
✅ Requisito 1 - Criar Classe Usuario
A classe Usuario.java deve conter os seguintes atributos:
pkidusu (int)
nomeusu (String)
emailusu (String)
senhausu (String)
foneusu (String)
cpfusu (String)
enderecousu (String)
Crie os métodos:
// Construtor padrão e completo
public Usuario(int id, String nome, String email, String senha, String fone, String cpf, String endereco) {}

// Getters e Setters
public int getId() {}
public void setId(int id) {}
// ... outros getters e setters
✅ Requisito 2 - Implementar Sistema de Login
Criar uma tela de login (FrmLogin.java).
Implementar método para validar o login:
public boolean validarLogin(String email, String senha) {
    // Lógica para verificar se o email e senha existem no banco
}
Se o usuário não existir, abrir tela de cadastro (FrmCadUsuario.java).
✅ Requisito 3 - Validar Senha Forte
Crie um método na classe Usuario para validar a senha.
A senha deve ter no mínimo 8 caracteres e conter pelo menos:
Uma letra maiúscula
Uma letra minúscula
Um número
Um caractere especial (@, #, $, %, etc.)
O que fazer:
Crie um método chamado validarSenha(String senha) que retorna um boolean.
Use o método matches() com expressões regulares (regex) para validar.
✅ Requisito 4 - Confirmar Senha
Ao cadastrar o usuário, peça para o usuário digitar a senha duas vezes para confirmação.
Se as senhas não forem iguais, exiba uma mensagem de erro.
✅ Requisito 5 - Criar Tela de Cadastro de Usuário
Criar FrmCadUsuario.java para permitir cadastro de usuário.
Chamar o método salvar() na DAO ao clicar em salvar.
✅ Requisito 6 - Salvar Usuário no Banco de Dados
Implementar o método salvar() na UsuarioDAO.java:
public void salvar(Usuario usuario) {
    // Código para salvar no banco de dados
}
✅ Requisito 7 - Validar CPF
Crie um método na classe Usuario para validar o CPF.
O método deve verificar se o CPF é válido (formato e dígitos verificadores).
Exemplo:
public boolean validarCPF(String cpf) {
    // Implementação da validação de CPF
}
🐶 Pet
✅ Requisito 1 - Criar Classe Pet
A classe Pet.java deve conter os seguintes atributos:
id (int)
nomePet (String)
raca (String)
anoNascimento (int)
sexo (String)
corPelo (String)
Crie os métodos:
// Construtor padrão e completo
public Pet(int id, String nomePet, String raca, int anoNascimento, String sexo, String corPelo) {}

// Getters e Setters
public int getId() {}
public void setId(int id) {}
✅ Requisito 2 - Criar Tela de Cadastro de Pet
Criar FrmCadPet.java para permitir cadastro de pet.
Chamar o método salvar() na DAO ao clicar em salvar.
✅ Requisito 3 - Salvar Pet no Banco de Dados
Implementar o método salvar() na PetDAO.java:
public void salvar(Pet pet) {
    // Código para salvar no banco de dados
}

git clone https://github.com/seu-usuario/seu-repositorio.git
cd seu-repositorio
Configure o MySQL

Inicie o XAMPP e ative o serviço MySQL
Acesse o phpMyAdmin (http://localhost/phpmyadmin)
Crie um banco de dados chamado cadastro_pet
Execute os scripts SQL fornecidos na seção "Banco de Dados"
Configure o projeto no NetBeans

Abra o NetBeans IDE
Vá para "File" > "Open Project" e selecione a pasta do projeto
Certifique-se de que as bibliotecas Java necessárias estão incluídas (MySQL Connector/J)
Compile e execute o projeto

Clique com o botão direito no projeto e selecione "Clean and Build"
Execute o projeto clicando em "Run" ou pressionando F6
📅 Cronograma Sugerido
Semana	Atividade
Dia 1	Configuração do ambiente e banco de dados - Implementação das classes de entidade (Usuario e Pet)
Dia 2	Implementação das classes DAO - Criação das interfaces gráficas
Dia 3	Testes e correção de bugs
Dia 4	Apresentação do projeto
🤝 Contribuição e Suporte
Para dúvidas ou sugestões sobre o projeto, entre em contato com Bruno Model Martinho



