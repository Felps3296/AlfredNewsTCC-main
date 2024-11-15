# 📰 **Sistema de Notícias Personalizado com Power Platform**

## 📚 **Descrição do Projeto**
Este projeto tem como objetivo criar um sistema na plataforma **Power Platform**, utilizando ferramentas e serviços modernos para oferecer uma experiência personalizada de consumo de notícias. O sistema combina APIs e inteligência artificial para fornecer informações simplificada, adaptada aos interesses do usuário e integrada com dispositivos habilitados para **Alexa**.

---

## 🚀 **Principais Funcionalidades**
- 🌐 **Busca de Notícias Personalizadas:** Integração com a **News API** para buscar notícias com base nos interesses registrados pelos usuários.  
- 🤖 **Resumo com Inteligência Artificial:** Uso da **API do ChatGPT** para formatar as notícias de forma reduzida, simples e atrativa.  
- 🗣️ **Integração com Alexa:** Desenvolvimento de uma **Skill Alexa** que lê as notícias simplificadas para os usuários.  
- 📱 **Aplicativo Interativo:** Permite que o usuário registre suas preferências de notícias em um banco de dados centralizado (**Dataverse**).

---

## 🛠️ **Tecnologias e Ferramentas Utilizadas**
### 🌟 **Plataforma**
- **Power Platform**: Serviço **PaaS** utilizado para desenvolvimento do sistema.

### 🔧 **APIs e Integrações**
- **News API**: Coleta de notícias com base em categorias e interesses.  
- **OpenAI ChatGPT API**: Resumo das notícias com inteligência artificial.  
- **Power Automate**: Orquestração das chamadas de APIs e automações.  
- **Amazon Alexa Skill**: Integração para leitura das notícias por meio de dispositivos habilitados.

### 📦 **Banco de Dados**
- **Microsoft Dataverse**: Armazenamento centralizado dos dados de preferências dos usuários.

---
## 📋 **Como Configurar e Utilizar**

### Configuração do Ambiente
- Acesse a **Power Platform** e configure um ambiente com suporte ao **Dataverse**.
- Habilite o uso do **Power Automate** para integrações.

### Configuração das APIs
- Crie uma conta e obtenha a chave de acesso para a **News API**.
- Configure a integração com a **API do ChatGPT** da OpenAI.

### Skill Alexa
- Crie uma Skill personalizada na plataforma da **Amazon Alexa**.
- Configure a Skill para consumir a API desenvolvida no **Power Automate**.

### Deploy do Aplicativo
- Utilize o aplicativo criado para registrar preferências e consultar notícias.

<h2>✍️ Autor</h2>

<a href="https://github.com/Felps3296">
  <img loading="lazy" src="https://avatars.githubusercontent.com/u/64935845?v=4" width="115" alt="Felipe Viana Reis">
</a>
<br>
<sub><b>Felipe Viana Reis</b></sub>
<br>

## 📐 **Arquitetura do Sistema**
```mermaid
graph LR
A[📱 Usuário] -->|Registra preferências| B[📦 Dataverse]
B -->|Consulta preferências| C[🌐 News API]
C -->|Recebe notícias| D[🤖 ChatGPT API]
D -->|Notícia formatada| E[🗣️ Alexa Skill]
E -->|Consulta APIs| F[🔧 Power Automate]
