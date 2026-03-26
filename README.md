# 🎙️ Voice-AI-Automations: Speech-to-Action Hub

Este repositório é um laboratório de automação inteligente focado em **Interfaces de Voz (VUI)**. O objetivo é demonstrar como integrar modelos de processamento de áudio (STT) e modelos de linguagem de baixa latência (LLMs) para transformar a fala humana em ações digitais concretas e automações de produtividade.

O ecossistema utiliza uma arquitetura de múltiplos agentes para garantir precisão, velocidade e utilidade real no dia a dia.

---

## 🚀 Projetos no Repositório

### 1. 🏗️ Projeto Base: Voice-to-LLM (Whisper + Gemini)
O "esqueleto" fundamental do hub. Uma estrutura robusta que capta áudio do microfone, realiza a transcrição precisa e processa uma resposta inteligente.
- **Destaque:** Base para entender a orquestração entre hardware (microfone) e APIs de IA.

### 2. 📊 SQL Voice Assistant (Text-to-SQL)
Um assistente de banco de dados que permite realizar consultas complexas em linguagem natural, ideal para análise de dados rápida.
- **Funcionalidade:** Traduz comandos como *"Quais são os 10 produtos mais caros?"* para `SELECT * FROM produtos ORDER BY preco DESC LIMIT 10`.
- **Tecnologias:** SQLite, Pandas, **Groq (Llama 3.1)** e Whisper.

### 3. 📝 Assistente de Reuniões Inteligente (Voice-to-PDF)
Automatização de processos administrativos que escuta diálogos, resume pontos-chave e gera documentos profissionais instantaneamente.
- **Funcionalidade:** Analisa a transcrição da reunião, extrai tópicos, decisões e planos de ação, exportando tudo para um arquivo **PDF formatado**.
- **Tecnologias:** **Groq (Llama 3.1)**, FPDF e Whisper.

---

## 🛠️ Stack Técnica

Para garantir performance e latência mínima, o projeto utiliza:

* **STT (Speech-to-Text):** `OpenAI Whisper` para transcrição local de alta fidelidade.
* **LLM (Cérebro):** `Llama 3.1` via **Groq Cloud** para processamento de intenções e síntese de texto com velocidade extrema.
* **TTS (Text-to-Speech):** `gTTS` para feedback audível das ações realizadas pela IA.
* **Manipulação de Dados:** `Pandas` e `SQLite`.
* **Geração de Documentos:** `FPDF`.

---

## ⚙️ Como Executar

1.  Abra os arquivos `.ipynb` no **Google Colab**.
2.  Configure suas chaves de API nos "Secrets" do Colab (ícone de chave na lateral esquerda):
    * `GROQ_API_KEY`
    * `GEMINI_API_KEY` (utilizada no projeto base)
3.  Execute as células em ordem e utilize o microfone do seu navegador quando solicitado para enviar os comandos por voz.

---
