# n8n Workflows — Luan Taraschi

[![License: MIT](https://img.shields.io/badge/License-MIT-0b1220.svg?style=for-the-badge&labelColor=0b1220&color=64ffda)](LICENSE)
![Stack](https://img.shields.io/badge/n8n-Workflows-64ffda?style=for-the-badge&labelColor=0b1220)

Coleção de **workflows n8n** focados em **automação com IA e integrações** (Gmail, Google Drive, APIs, webhooks).  
Todos os arquivos **não** contêm credenciais. Use suas chaves via **Credenciais do n8n** ou **variáveis de ambiente** (veja `.env.example`).

---

## 🧭 Sumário

- [O que você encontra aqui](#-o-que-você-encontra-aqui)
- [Como usar](#-como-usar)
- [Workflows](#-workflows)
- [Variáveis de ambiente](#-variáveis-de-ambiente)
- [Rodar local com Docker](#-rodar-local-com-docker)
- [Segurança](#-segurança)
- [Estrutura do repositório](#-estrutura-do-repositório)
- [Sobre](#-sobre)
- [Licença](#-licença)

---

## ✨ O que você encontra aqui

- Workflows prontos para importar, com foco em:
  - **Atendimento/Chatbots**, **Geração de Conteúdo**, **Produtividade** (Calendário), **Roteamento de E-mails)
- **Boas práticas de segurança** (sem segredos no repositório)
- **Pré-visualizações** (prints/GIFs) para entender cada fluxo antes de importar
- Instruções simples para **rodar localmente** (Docker) e **importar via interface** ou **CLI**

---

## 🚀 Como usar

### Importar pela interface (recomendado)
1. Abra seu **n8n** (Cloud ou local).  
2. Vá em **Workflows → Import from file**.  
3. Selecione o arquivo `.json` do workflow na pasta `workflows/`.

### Importar pela CLI (opcional)
```bash
# importar um workflow específico
npx n8n import:workflow --input ./workflows/<nome-do-workflow>.json

# importar todos (bash)
for f in ./workflows/*.json; do npx n8n import:workflow --input "$f"; done
