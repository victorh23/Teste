<h1 align="center">Sistema de Gerenciamento de Usuários</h1>
<p align="center"> Um sistema de gerenciamento de usuários contendo cadastro, autenticação, validação de senhas e lista de usuários. Apenas os usuários logados podem visualizar suas próprias informações e somente administradores podem visualizar informações de todos os usuários. Os usuários podem alterar suas senhas na tela de login se esquecerem.</p>
</br>


Tecnologias e técnicas :

- [ExpressJS](https://expressjs.com/)
- [React](https://pt-br.reactjs.org/),
- [React Router DOM](https://reactrouter.com/docs/en/v6/getting-started/overview),
- [Redux](https://redux.js.org/),
- [Styled components](https://styled-components.com/),
- [Node.js](https://nodejs.org/pt-br/),
- [MySql](https://www.mysql.com),
- [Sequelize](https://sequelize.org/),
- [Nodemon](https://www.npmjs.com/package/nodemon),
- [Json Web Token](https://jwt.io/),
- [BCRYPT](https://www.npmjs.com/package/bcrypt),
- [CORS](https://www.npmjs.com/package/cors),
- [YUP](https://www.npmjs.com/package/yup),
- [React-Toastify](https://npm.io/package/react-toastify)

</br>

### Caracteristicas do projeto

-  Cadastro de usuários
-  Autenticação de usuários
-  Criptografia de senha
-  Validação de dados de cadastro
-  Gerenciamento de usuários
-  Listagem de usuários
-  Exclusão de usuários (_Administradores_)
-  Alteração de senhas

</br></br>


## Requisitos

Antes de começar, você precisará ter na sua maquina:
</br>


- Node js
- MySQL


## Iniciando o Projeto


```bash
# Clone este repositório
$ git clone <https://github.com/victorh23/teste.git>

# Acesse a pasta do backend
$ cd backend

# Instale as dependências
$ npm install

# Inicie a aplicação
$ npm run app

### Iniciando o Front End

# Retorne para a pasta front-end
$ cd -

# Acesse a pasta do frontend
$ cd frontend

# Instale as dependências
$ npm install

# Inicie a aplicação
$ npm run dev

```

## Configurando o Banco de Dados

- Instale o MySQL versão 8 ou mais nova como SERVER ONLY, selecionando o tipo de configuração como "Development ". Mantenha a porta padrão 3306 e forneça a senha "1234". Finalize a instalação.

- Se você estiver usando o Windows, vá até o diretório C > Arquivos de Programas > MySQL > BIN e copie a URL da pasta. Em seguida, clique com o botão direito do mouse no Meu Computador, vá em Propriedades, Configurações Avançadas do Sistema e adicione a URL copiada às variáveis de ambiente PATH.

- Abra o Prompt de Comando ou outro programa similar e digite `mysql -h localhost -u root -p`, pressionando enter. Será solicitada a senha "1234". Após inserir a senha, você estará dentro do MySQL.

__Recomendo executar o comando `create database cadastrodeusuarios` para criar a tabela de cadastro de usuários e evitar alterações no back-end.__

```
- # Acesse a pasta do backend
$ cd backend

# Execute as migrations
$ npx sequelize-cli db:migrate

// Para criar a tabela "users" dentro do banco "cadastrodeusuarios". E em seguida.

# Execute o seed
$ npx sequelize db:seed:all

// Para já adicionar o usuário ADMIN na tabela.

```

- Agora você já pode realizar o cadastro de usuários e fazer as operações de gerenciamento de usuários através da aplicação.


## Considerações 

- Voce tem que se certificar de que o serviço do MySQL esteja iniciado antes de iniciar a aplicação.
- Caso seja necessario, altere as configurações de segurança do MySQL para permitir a conexão local.
- Não esqueça de configurar as variaveis de ambiente necessárias.
- Lembre-se que o usuário pode se cadastrar, porém ao fazer login, somente poderá visualizar as informações dele mesmo. Para visualizar todos os usuários cadastrados, é necessário ser admin.
- É possível para o usuário alterar sua senha através da tela de login.





