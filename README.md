# n8n Workflows — Luan Taraschi

Coleção de workflows n8n focados em automação com IA e integrações (OpenAI, WhatsApp, e-mail, calendário).  
Os arquivos **não** contêm credenciais. Use suas chaves via **Credenciais do n8n** ou variáveis de ambiente (veja `.env.example`).

## 🚀 Como usar

### Importar pela interface
1. Abra seu n8n (Cloud ou local).
2. **Workflows → Import from file** e selecione um `.json` da pasta `workflows/`.

### Importar pela CLI
```bash
# importar um único
npx n8n import:workflow --input ./workflows/bots-whatsapp.json

# importar todos (bash)
for f in ./workflows/*.json; do npx n8n import:workflow --input "$f"; done
