# ✂️ Sistema de Barbearia - Desktop App

Uma aplicação desktop moderna para gerenciamento de serviços e controle de acessos de uma barbearia. Desenvolvida em Python, a interface utiliza componentes visuais elegantes e conta com um banco de dados relacional robusto para o armazenamento seguro das informações.

---

## 🚀 Funcionalidades

* **Autenticação Segura:** Sistema de login e cadastro com senhas criptografadas.
* **Níveis de Acesso:** Redirecionamento automático baseado no tipo de usuário:
  * **Cliente:** Visualização simples e limpa da tabela de serviços e preços atualizados.
  * **Administrador:** Painel exclusivo para cadastro, monitoramento e gerenciamento de novos serviços em tempo real.
* **Interface Responsiva:** Desenvolvida em Modo Escuro (*Dark Mode*) nativo.

---

## 📸 Demonstração do Sistema

### 🔐 Tela de Login e Cadastro
Interface inicial onde os clientes realizam o acesso ou criam uma nova conta no banco de dados.
<img width="600" height="650" alt="image" src="https://github.com/user-attachments/assets/43c4b183-7a9d-4e17-b9cf-7fc63d8da394" />



### 👥 Painel do Cliente
Área destinada aos clientes para consulta da tabela de preços e serviços oferecidos pela barbearia.
<img width="750" height="801" alt="image" src="https://github.com/user-attachments/assets/acc78b8e-4ecb-4907-ae45-3efba3892d10" />


### ⚙️ Painel do Administrador
Área de gerenciamento exclusiva, permitindo a inserção de novos serviços e atualização instantânea da lista.
<img width="749" height="794" alt="image" src="https://github.com/user-attachments/assets/e713b3d1-948d-4aef-b7e7-8f2ed427d580" />

---

## 🛠️ Tecnologias Utilizadas

* **[Python](https://www.python.org/):** Linguagem base do projeto.
* **[CustomTkinter](https://github.com/TomSchimansky/CustomTkinter):** UI library baseada no Tkinter para criação de interfaces modernas e customizáveis.
* **[PostgreSQL](https://www.postgresql.org/):** Banco de dados relacional para persistência de dados.
* **[Bcrypt](https://pypi.org/project/bcrypt/):** Criptografia de senhas utilizando técnicas de *hashing* seguras.
* **[Psycopg2](https://pypi.org/project/psycopg2/):** Adaptador de banco de dados PostgreSQL para Python.
* **[Python-dotenv](https://pypi.org/project/python-dotenv/):** Gerenciamento de variáveis de ambiente para proteção de credenciais.

---

## 🔧 Configuração e Instalação

### Pré-requisitos
* Python 3.x instalado.
* Instância do banco de dados PostgreSQL ativa (local ou em nuvem).

### 1. Clonar o Repositório
```bash
git clone [https://github.com/seu-usuario/sistema-barbearia.git](https://github.com/seu-usuario/sistema-barbearia.git)
cd sistema-barbearia
2. Instalar as Dependências
Instale as bibliotecas necessárias listadas no projeto:

Bash
pip install customtkinter psycopg2-binary bcrypt python-dotenv
3. Variáveis de Ambiente
Crie um arquivo chamado .env na raiz do projeto e preencha com as credenciais do seu banco de dados PostgreSQL:

Snippet de código
DB_HOST=seu_host_aqui
DB_USER=seu_usuario_aqui
DB_PASS=sua_senha_aqui
DB_NAME=seu_nome_do_banco_aqui
DB_PORT=5432
4. Executar o Aplicativo
Bash
python main.py
🔒 Segurança de Dados
O sistema preza pela segurança das credenciais dos usuários. Ao realizar o cadastro, a senha fornecida nunca é salva em texto puro no banco de dados. É gerada uma chave aleatória (salt) e aplicada uma função de criptografia via Bcrypt, garantindo que apenas hashes seguros fiquem armazenados no PostgreSQL.

📄 Licença
Este projeto está sob a licença MIT. Veja o arquivo LICENSE para mais detalhes.
