# n8n Workflows — Luan Taraschi

Coleção de **workflows n8n** focados em **automação com IA e integrações** (Gmail, Google Drive, APIs externas, webhooks).  
Todos os arquivos **não** contêm credenciais. Use as suas via **Credenciais do n8n** ou variáveis de ambiente (veja `.env.example`).

---

## ✨ O que você encontra aqui

- Workflows prontos para importar, com foco em:
  - **Atendimento/Chatbots**, **Geração de Conteúdo**, **Produtividade** (Calendário), **Roteamento de E-mails**.
- **Boas práticas de segurança** (sem segredos no repositório).
- **Pré-visualizações** (prints/GIFs) para entender cada fluxo antes de importar.
- Instruções simples para **rodar localmente** (Docker) e **importar via interface** ou **CLI**.

---

## 🚀 Como usar

### Importar pela interface (recomendado)
1. Abra seu n8n (Cloud ou local).
2. Vá em **Workflows → Import from file**.
3. Selecione o arquivo `.json` do workflow na pasta `workflows/`.

### Importar pela CLI (opcional)
```bash
# importar um workflow específico
npx n8n import:workflow --input ./workflows/<nome-do-workflow>.json

# importar todos (bash)
for f in ./workflows/*.json; do npx n8n import:workflow --input "$f"; done
