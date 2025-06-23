# 🎥 Apresentação da Equipe Devflow e Instalação de Software
🔗 [Link do Vídeo](https://youtu.be/uV6GRuS7C3M)

## 🧠 Introdução ao Projeto
A equipe Devflow é composta por alunos do primeiro semestre do curso de Desenvolvimento de Software Multiplataforma.
Nosso objetivo é relatar as atividades realizadas no laboratório 103, incluindo a instalação de sistemas e softwares essenciais para o desenvolvimento.

## 💿 1. Instalação do Linux
Instalamos o Linux em quatro máquinas do laboratório. Utilizamos uma distribuição baseada em Debian (como o Ubuntu).
Etapas:

- Criar pendrive bootável com Rufus (Windows) ou dd (Linux).

- Iniciar o computador pelo pendrive.

- Seguir o instalador gráfico até a finalização.

## 💻 2. Instalação do VS Code

A instalação do VS Code foi feita **via interface gráfica**, sem necessidade de utilizar o terminal.

### 📥 Etapas realizadas:

- Acessamos o site oficial do Visual Studio Code:  
   [https://code.visualstudio.com/](https://code.visualstudio.com/)

- Selecionamos a versão `.deb` para distribuições baseadas em Debian (como o Ubuntu).

- Após o download, **abrimos o arquivo com o instalador padrão do sistema**.

- O sistema cuidou da instalação automaticamente.

- Após a conclusão, o VS Code ficou disponível no menu de aplicações.

## 🐘 3. Instalação do PostgreSQL
O PostgreSQL foi instalado via terminal. Abaixo os comandos utilizados.

🔧 Comandos:
```bash
# Atualizar os pacotes:
sudo apt update

# Instalar PostgreSQL e o cliente:
sudo apt install postgresql postgresql-contrib

# Verificar o status do serviço:
sudo systemctl status postgresql

# Acessar como usuário postgres:
sudo -i -u postgres
psql

# Criar novo usuário (exemplo):
CREATE USER meuusuario WITH PASSWORD 'minhasenha';
```

## 🐘 3.1 Instalação do pgAdmin

O **pgAdmin** é uma ferramenta gráfica para gerenciar bancos de dados PostgreSQL, facilitando a visualização, criação de tabelas, execução de queries e muito mais.

### 📥 Etapas de instalação:

1. Adicionamos o repositório oficial do pgAdmin 4:

```bash
# Instalar dependências:
sudo apt install curl ca-certificates gnupg

# Importar a chave pública do repositório:
curl https://www.pgadmin.org/static/packages_pgadmin_org.pub | sudo gpg --dearmor -o /usr/share/keyrings/pgadmin-keyring.gpg

# Adicionar o repositório:
echo "deb [signed-by=/usr/share/keyrings/pgadmin-keyring.gpg] https://ftp.postgresql.org/pub/pgadmin/pgadmin4/apt/$(lsb_release -cs) pgadmin4 main" | sudo tee /etc/apt/sources.list.d/pgadmin4.list

# Atualizar os pacotes:
sudo apt update
```

## 🟢 4. Instalação do Node.js
Instalamos o Node.js diretamente do repositório oficial NodeSource para garantir a versão LTS.

⚙️ Comandos:
```bash
# Atualizar pacotes:
sudo apt update

# Instalar curl:
sudo apt install curl

# Baixar e executar o script de setup do Node.js:
curl -fsSL https://deb.nodesource.com/setup_20.x | sudo -E bash -

# Instalar Node.js:
sudo apt install -y nodejs

# Verificar versões:
node -v
npm -v
```

## 🌐 5. Deploy do Projeto da ABP
O projeto da ABP foi apresentado com frontend e backend já implantados.
O site está disponível online, o que facilitou a apresentação sem precisar abrir o código no VS Code.

## 📚 Funcionalidades do Site
Consulta dos cursos da FATEC Jacareí

Visualização das grades curriculares

Filtro por período letivo

## ✅ Conclusão
A equipe concluiu a instalação de ferramentas fundamentais para o desenvolvimento de software.
A maioria das ferramentas foi instalada via terminal, exceto o VS Code, que teve um processo gráfico simplificado.
A experiência no laboratório 103 foi essencial para nosso aprendizado prático.

## 🗣️ Considerações Finais
A equipe Devflow está satisfeita com os resultados alcançados e com o funcionamento dos sistemas instalados.
Continuamos motivados a aprimorar nossas habilidades e enfrentar os próximos desafios do curso com entusiasmo.

