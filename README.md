# 📚 Projeto Flask

## 📌 Descrição

Este projeto foi desenvolvido como trabalho final da disciplina de Introdução à Programação (IP). Trata-se de uma aplicação web construída com Flask que combina um sistema de glossário com integração à inteligência artificial do Google Gemini.

O sistema permite gerenciar termos e definições (CRUD completo) utilizando persistência em arquivo CSV, além de oferecer uma funcionalidade de perguntas e respostas com IA.

---

## 🎯 Objetivos

* Aplicar conceitos fundamentais de programação
* Desenvolver uma aplicação web com Flask
* Implementar operações de CRUD
* Manipular arquivos CSV para persistência de dados
* Integrar uma API de inteligência artificial (Google Gemini)
* Trabalhar com rotas, templates e formulários

---

## ⚙️ Funcionalidades

### 📖 Glossário (CRUD)

* ✅ Adicionar novos termos e definições
* 🔍 Listar todos os termos cadastrados
* ✏️ Editar termos existentes
* ❌ Remover termos
* 💾 Armazenamento em arquivo `bd_glossario.csv`

### 🤖 Integração com IA (Gemini)

* Envio de perguntas via formulário
* Geração de respostas utilizando o modelo `gemini-2.0-flash`
* Tratamento de erros de requisição

### 🌐 Páginas do sistema

* Página inicial (`/`)
* Sobre a equipe (`/sobre-equipe`)
* Fundamentos (`/fundamentos`)
* Glossário (`/glossario`)
* Cadastro de novo termo (`/novo_termo`)
* Integração com IA (`/gemini`)

---

## 🛠️ Tecnologias utilizadas

* Python
* Flask
* CSV (armazenamento de dados)
* Google Generative AI (Gemini API)
* HTML / CSS (templates)

---

## 📂 Estrutura do Projeto

Projeto_Final_ip_cc/
│
├── app.py
├── templates/
│   ├── index.html
│   ├── sobre.html
│   ├── fundamentos.html
│   ├── glossario.html
│   ├── novo_termo.html
│   └── gemini.html
├── static/
├── bd_glossario.csv
├── .env
└── README.md

---

## 🚀 Como executar o projeto

1. Clone o repositório:
   git clone https://github.com/Brunoapf/Projeto_Final_ip_cc.git

2. Acesse a pasta:
   cd Projeto_Final_ip_cc

3. Instale as dependências:
   pip install flask google-generativeai python-dotenv

4. Configure a API do Gemini:
   Crie um arquivo `.env` na raiz do projeto e adicione:
   GEMINI_API_KEY=sua_chave_aqui

5. No código, substitua:
   genai.configure(api_key="Your Geminiai api key")
   por:
   genai.configure(api_key=os.getenv("GEMINI_API_KEY"))

6. Execute o projeto:
   python app.py

7. Acesse no navegador:
   http://localhost:5000

---

## 📸 Demonstração

(Adicione prints do sistema: glossário, formulário e integração com IA)

---

## 📖 Conceitos aplicados

* Estruturas condicionais
* Laços de repetição
* Manipulação de arquivos CSV
* Funções e organização de código
* CRUD (Create, Read, Update, Delete)
* Desenvolvimento web com Flask
* Integração com APIs externas

---

## 👨‍💻 Autor

Bruno De Araújo

---

## 📌 Observações

Este projeto tem fins educacionais e foi desenvolvido como parte da disciplina de Introdução à Programação. A integração com o Google Gemini depende de uma chave de API válida.
