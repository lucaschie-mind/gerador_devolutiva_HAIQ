# HAI-Q Dashboard

Painel de acompanhamento de candidatos do assessment HAI-Q.

## Deploy no Railway

1. Crie um **novo repositório** no GitHub com os arquivos desta pasta
2. No Railway → New Project → Deploy from GitHub repo
3. Adicione as variáveis de ambiente:
   - `DATABASE_URL` — mesma do projeto principal (PostgreSQL)
   - `HAIQ_BASE_URL` — URL do assessment (ex: https://assessmenthaiq-production.up.railway.app)
4. Railway detecta o Procfile e sobe o Streamlit automaticamente

## Variáveis de ambiente

| Variável | Descrição |
|----------|-----------|
| `DATABASE_URL` | Connection string do PostgreSQL Railway |
| `HAIQ_BASE_URL` | URL base do app de assessment |

## Uso

- **Upload de Excel/CSV**: envie um arquivo com coluna `email`
- **Digitar manualmente**: cole os e-mails, um por linha
- Clique em **Buscar status** para ver os resultados
- Baixe o Excel com os resultados e links clicáveis
