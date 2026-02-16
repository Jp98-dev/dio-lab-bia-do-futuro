# 🛡️ Guardião - O Educador Financeiro

> Um agente inteligente de educação financeira alimentado por IA Generativa

## 📋 Sobre o Projeto

O **Guardião** é um assistente financeiro inteligente projetado para educar e empoderar pessoas em sua jornada de educação financeira. Diferente de chatbots tradicionais, o Guardião atua de forma proativa, personalizando orientações com base no perfil e histórico de cada usuário.

### 🎯 Objetivo

Democratizar o acesso à educação financeira através de um agente conversacional que:
- Ensina conceitos financeiros de forma didática
- Adapta a linguagem ao nível de conhecimento do usuário
- Fornece orientações personalizadas baseadas em dados reais
- Promove decisões financeiras conscientes e informadas

## ✨ Funcionalidades

- **📚 Educação Personalizada**: Conteúdo adaptado ao nível de conhecimento do usuário
- **💡 Análise Inteligente**: Avaliação de perfil e histórico de transações
- **🎓 Mentoria Financeira**: Orientações sobre investimentos, economia e planejamento
- **📊 Insights Proativos**: Identificação de padrões e sugestões de melhoria
- **🔒 Respostas Confiáveis**: Sistema anti-alucinação para garantir informações precisas

## 🏗️ Arquitetura

```
┌─────────────────┐
│   Interface     │  (Streamlit/Gradio)
│   do Usuário    │
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│   Orquestrador  │  (LangChain/CrewAI)
│   de Agentes    │
└────────┬────────┘
         │
    ┌────┴────┬────────────┐
    ▼         ▼            ▼
┌────────┐ ┌─────┐  ┌──────────┐
│  LLM   │ │Data │  │ Prompts  │
│(GPT/   │ │Base │  │Engineering│
│Claude) │ │     │  │          │
└────────┘ └─────┘  └──────────┘
```

## 📂 Estrutura do Projeto

```
guardiao-educador-financeiro/
│
├── 📄 README.md                      # Este arquivo
├── 📄 README.pt-BR.md               # Versão em português
│
├── 📁 data/                          # Base de conhecimento
│   ├── transacoes.csv               # Histórico de transações
│   ├── historico_atendimento.csv    # Histórico de interações
│   ├── perfil_investidor.json       # Perfil do usuário
│   └── produtos_financeiros.json    # Produtos disponíveis
│
├── 📁 docs/                          # Documentação detalhada
│   ├── 01-documentacao-agente.md    # Arquitetura e caso de uso
│   ├── 02-base-conhecimento.md      # Estratégia de dados
│   ├── 03-prompts.md                # Engenharia de prompts
│   ├── 04-metricas.md               # Avaliação e métricas
│   └── 05-pitch.md                  # Apresentação do projeto
│
├── 📁 src/                          # Código fonte
│   ├── app.py                       # Aplicação principal
│   ├── agent/                       # Lógica do agente
│   ├── prompts/                     # Templates de prompts
│   └── utils/                       # Utilitários
│
└── 📁 examples/                     # Exemplos de uso
    └── conversas_exemplo.md
```

## 🚀 Como Usar

### Pré-requisitos

- Python 3.8+
- Conta em provedor de LLM (OpenAI, Anthropic, Google, etc.)
- pip ou conda para gerenciar dependências

### Instalação

```bash
# Clone o repositório
git clone https://github.com/Jp98-dev/dio-lab-bia-do-futuro.git
cd dio-lab-bia-do-futuro

# Crie um ambiente virtual
python -m venv venv
source venv/bin/activate  # Linux/Mac
# ou
venv\Scripts\activate  # Windows

# Instale as dependências
pip install -r requirements.txt

# Configure suas variáveis de ambiente
cp .env.example .env
# Edite .env com suas credenciais
```

### Execução

```bash
# Inicie a aplicação
streamlit run src/app.py

# Ou utilize o notebook de exemplo
jupyter notebook examples/demo.ipynb
```

## 🛠️ Tecnologias Utilizadas

- **IA Generativa**: GPT-4, Claude, ou Gemini
- **Framework**: LangChain / CrewAI
- **Interface**: Streamlit / Gradio
- **Dados**: Pandas, JSON
- **Versionamento**: Git/GitHub

## 📊 Exemplos de Interação

**Usuário**: "Quanto posso gastar esse mês sem comprometer meus objetivos?"

**Guardião**: "Com base no seu histórico, você tem R$ 2.500 de renda mensal. Considerando suas despesas fixas de R$ 1.800 e sua meta de poupar 20% para investimentos (R$ 500), recomendo limitar gastos variáveis a R$ 200. Isso garante folga para imprevistos e mantém você no caminho das suas metas! 💰"

---

**Usuário**: "Devo investir em ações agora?"

**Guardião**: "Seu perfil indica moderação ao risco. Antes de ações, vamos garantir que você tenha uma reserva de emergência de 6 meses de despesas (cerca de R$ 10.800). Você já tem R$ 3.000 guardados. Que tal focarmos em completar essa reserva primeiro em ativos de baixo risco? Depois podemos explorar ações! 📈"

## 🔒 Segurança e Privacidade

- ✅ Dados sensíveis são mockados/anonimizados
- ✅ Sistema anti-alucinação para respostas confiáveis
- ✅ Validação de informações financeiras críticas
- ✅ Respeito às diretrizes de proteção de dados

## 🎯 Roadmap

- [ ] Integração com Open Banking
- [ ] Análise preditiva de gastos
- [ ] Gamificação da educação financeira
- [ ] Suporte a múltiplos idiomas
- [ ] App mobile nativo

## 🤝 Contribuindo

Contribuições são bem-vindas! Sinta-se à vontade para:

1. Fazer um Fork do projeto
2. Criar uma branch para sua feature (`git checkout -b feature/MinhaFeature`)
3. Commit suas mudanças (`git commit -m 'Adiciona MinhaFeature'`)
4. Push para a branch (`git push origin feature/MinhaFeature`)
5. Abrir um Pull Request

## 📝 Licença

Este projeto foi desenvolvido como parte do bootcamp da [Digital Innovation One](https://www.dio.me/).

## 👨‍💻 Autor

Desenvolvido por **[Jp98-dev](https://github.com/Jp98-dev)**

---

⭐ Se este projeto te ajudou, considere dar uma estrela!

🔗 [LinkedIn](https://www.linkedin.com/in/seu-perfil) | [Portfolio](https://seu-portfolio.com)

# 🛡️ Guardian - The Financial Educator

> An intelligent financial education agent powered by Generative AI

[Português](README.pt-BR.md) | **English**

## 📋 About the Project

**Guardian** is an intelligent financial assistant designed to educate and empower people on their financial education journey. Unlike traditional chatbots, Guardian acts proactively, personalizing guidance based on each user's profile and history.

### 🎯 Objective

Democratize access to financial education through a conversational agent that:
- Teaches financial concepts in a didactic way
- Adapts language to the user's knowledge level
- Provides personalized guidance based on real data
- Promotes conscious and informed financial decisions

## ✨ Features

- **📚 Personalized Education**: Content adapted to the user's knowledge level
- **💡 Intelligent Analysis**: Profile and transaction history evaluation
- **🎓 Financial Mentoring**: Guidance on investments, savings, and planning
- **📊 Proactive Insights**: Pattern identification and improvement suggestions
- **🔒 Reliable Responses**: Anti-hallucination system to ensure accurate information

## 🏗️ Architecture

```
┌─────────────────┐
│   User          │  (Streamlit/Gradio)
│   Interface     │
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│   Agent         │  (LangChain/CrewAI)
│   Orchestrator  │
└────────┬────────┘
         │
    ┌────┴────┬────────────┐
    ▼         ▼            ▼
┌────────┐ ┌─────┐  ┌──────────┐
│  LLM   │ │Data │  │ Prompt   │
│(GPT/   │ │Base │  │Engineering│
│Claude) │ │     │  │          │
└────────┘ └─────┘  └──────────┘
```

## 📂 Project Structure

```
guardian-financial-educator/
│
├── 📄 README.md                      # This file
├── 📄 README.pt-BR.md               # Portuguese version
│
├── 📁 data/                          # Knowledge base
│   ├── transacoes.csv               # Transaction history
│   ├── historico_atendimento.csv    # Interaction history
│   ├── perfil_investidor.json       # User profile
│   └── produtos_financeiros.json    # Available products
│
├── 📁 docs/                          # Detailed documentation
│   ├── 01-documentacao-agente.md    # Architecture and use case
│   ├── 02-base-conhecimento.md      # Data strategy
│   ├── 03-prompts.md                # Prompt engineering
│   ├── 04-metricas.md               # Evaluation and metrics
│   └── 05-pitch.md                  # Project pitch
│
├── 📁 src/                          # Source code
│   ├── app.py                       # Main application
│   ├── agent/                       # Agent logic
│   ├── prompts/                     # Prompt templates
│   └── utils/                       # Utilities
│
└── 📁 examples/                     # Usage examples
    └── conversas_exemplo.md
```

## 🚀 Getting Started

### Prerequisites

- Python 3.8+
- LLM provider account (OpenAI, Anthropic, Google, etc.)
- pip or conda for dependency management

### Installation

```bash
# Clone the repository
git clone https://github.com/Jp98-dev/dio-lab-bia-do-futuro.git
cd dio-lab-bia-do-futuro

# Create a virtual environment
python -m venv venv
source venv/bin/activate  # Linux/Mac
# or
venv\Scripts\activate  # Windows

# Install dependencies
pip install -r requirements.txt

# Set up environment variables
cp .env.example .env
# Edit .env with your credentials
```

### Running

```bash
# Start the application
streamlit run src/app.py

# Or use the example notebook
jupyter notebook examples/demo.ipynb
```

## 🛠️ Technologies Used

- **Generative AI**: GPT-4, Claude, or Gemini
- **Framework**: LangChain / CrewAI
- **Interface**: Streamlit / Gradio
- **Data**: Pandas, JSON
- **Version Control**: Git/GitHub

## 📊 Interaction Examples

**User**: "How much can I spend this month without compromising my goals?"

**Guardian**: "Based on your history, you have $2,500 in monthly income. Considering your fixed expenses of $1,800 and your goal to save 20% for investments ($500), I recommend limiting variable expenses to $200. This ensures room for unexpected costs and keeps you on track with your goals! 💰"

---

**User**: "Should I invest in stocks now?"

**Guardian**: "Your profile indicates moderate risk tolerance. Before stocks, let's ensure you have an emergency fund of 6 months of expenses (about $10,800). You already have $3,000 saved. How about focusing on completing this reserve first with low-risk assets? Then we can explore stocks! 📈"

## 🔒 Security and Privacy

- ✅ Sensitive data is mocked/anonymized
- ✅ Anti-hallucination system for reliable responses
- ✅ Validation of critical financial information
- ✅ Compliance with data protection guidelines

## 🎯 Roadmap

- [ ] Open Banking integration
- [ ] Predictive spending analysis
- [ ] Financial education gamification
- [ ] Multi-language support
- [ ] Native mobile app

## 🤝 Contributing

Contributions are welcome! Feel free to:

1. Fork the project
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project was developed as part of [Digital Innovation One](https://www.dio.me/) bootcamp.

## 👨‍💻 Author

Developed by **[Jp98-dev](https://github.com/Jp98-dev)**

---

⭐ If this project helped you, consider giving it a star!

🔗 [LinkedIn](https://www.linkedin.com/in/your-profile) | [Portfolio](https://your-portfolio.com)
