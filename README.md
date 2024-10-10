# Blog de Postagens

Este é um projeto simples de um blog onde os usuários podem postar mensagens. Somente administradores podem ativar novos usuários. O primeiro usuário precisa ser ativado diretamente no banco de dados e promovido a administrador.

## Funcionalidades

- Criação de conta de usuário.
- Postagem de mensagens.
- Somente usuários ativos podem fazer login e postar mensagens.
- Somente administradores podem ativar novos usuários.
- O primeiro usuário deve ser ativado manualmente e promovido a administrador no banco de dados.

## Tecnologias utilizadas

- **Backend**: [PHP]
- **Frontend**: [HTML, CSS, JavaScript, etc.]
- **Banco de Dados**: [MySQL]

## Instalação

1. Clone o repositório:

   ```bash
   git clone https://github.com/seuusuario/blog-projeto.git
   cd blog-projeto
   ```

2. Instale as dependências do projeto:

   ```bash
   [Comando para instalar as dependências, por exemplo: pip install -r requirements.txt]
   ```

3. Configure o banco de dados no arquivo de configuração SQL Workbench.

4. Execute as migrações do banco de dados:

   ```bash
   [Comando para executar migrações, por exemplo: python manage.py migrate]
   ```

5. Crie o primeiro usuário no banco de dados e promova-o a administrador:

   - Acesse o banco de dados.
   - Localize a tabela de usuários e ative o primeiro usuário.
   - Promova o usuário à função de administrador alterando o campo de função.

   Exemplo de comandos SQL:

   ```sql
   UPDATE usuário SET ativo = 1;
   UPDATE usuário SET adm = 1;
   ```

6. Inicie o servidor:

   ```bash
   [Comando para iniciar o servidor, por exemplo: python manage.py runserver]
   ```

7. Acesse o blog no navegador:

   ```
   http://localhost:8000
   ```

## Como funciona

- Quando um novo usuário cria uma conta, ele estará inativo até que um administrador o ative.
- Somente administradores têm a permissão para ativar usuários.
- O primeiro usuário deve ser ativado manualmente e promovido a administrador diretamente no banco de dados.
- Administradores podem criar postagens e gerenciar os usuários.

## Contribuições

Contribuições são bem-vindas! Siga os passos abaixo para contribuir:

1. Faça um fork deste repositório.
2. Crie um branch com a sua feature (`git checkout -b minha-feature`).
3. Faça o commit das suas alterações (`git commit -m 'Adiciona minha feature'`).
4. Faça o push para o branch (`git push origin minha-feature`).
5. Abra um Pull Request.

## Licença

Este projeto está licenciado sob a MIT - consulte o arquivo LICENSE para mais detalhes.
