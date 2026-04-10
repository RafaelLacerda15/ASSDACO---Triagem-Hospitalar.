# 🏥 ASSDACO - Triagem Hospitalar (Ello's Brand)

**Micro SaaS para sistema de triagem hospitalar**  
Sistema completo de triagem desenvolvido como produto SaaS, com suporte nativo a **SQLite** (desenvolvimento local) e **PostgreSQL** (produção).  

Projeto que demonstra habilidades avançadas em backend Python: dual database strategy, migração automática de dados, deploy production-ready na Render e configuração profissional com Gunicorn.

---

### ✨ Principais Destaques

- 🔄 Suporte dual a bancos: **SQLite** (local) e **PostgreSQL** (produção)
- 🔄 Migração automática de dados do SQLite para PostgreSQL na primeira inicialização
- 🚀 Deploy pronto na Render com `render.yaml`
- 🛠️ Configuração production-grade com Gunicorn + variáveis de ambiente
- 🔐 Sistema de login administrativo seguro.
- 📊 Banco de dados de usuários e triagem totalmente separado e persistente

---

### 🛠️ Tecnologias Utilizadas

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=for-the-badge&logo=sqlite&logoColor=white)
![Gunicorn](https://img.shields.io/badge/Gunicorn-499848?style=for-the-badge&logo=gunicorn&logoColor=white)
![Render](https://img.shields.io/badge/Render-46E3B7?style=for-the-badge&logo=render&logoColor=white)

---

### 🚀 Quick Start

#### Ambiente Local (SQLite)

```bash
# 1. Clone o repositório
git clone https://github.com/RafaelLacerda15/assdaco-triagem.git
cd assdaco-triagem

# 2. Crie o arquivo de ambiente
cp .env.example .env

# 3. (Opcional) Deixe DATABASE_URL vazio para usar SQLite
# USERS_DATABASE_FILE=users.db
# TRIAGEM_DATABASE_FILE=triagem.db
# DATABASE_URL=

# 4. Instale as dependências e rode
pip install -r requirements.txt
python main.py
