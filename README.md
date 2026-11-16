# 🤖 Bot de Automação para WhatsApp

Automação em Python que lê uma planilha de clientes (nome, telefone e data de vencimento) e envia mensagens personalizadas pelo **WhatsApp Web**, incluindo links de pagamento.

![Python](https://img.shields.io/badge/Python-3.10+-3776AB?logo=python&logoColor=white)
![Status](https://img.shields.io/badge/status-funcional-success)

## ✨ Funcionalidades

- Leitura de clientes a partir de um arquivo `clientes.xlsx` (openpyxl)
- Mensagem personalizada com nome e data de vencimento
- Geração automática do link `web.whatsapp.com/send` para cada contato
- Clique automático no botão de envio com `pyautogui`
- Registro de falhas em `erros.csv` para reenvio posterior

## 🧰 Tecnologias

| Biblioteca | Uso |
|-----------|-----|
| `openpyxl` | Leitura da planilha Excel |
| `pyautogui` | Automação de mouse e teclado |
| `webbrowser` | Abertura do WhatsApp Web |
| `urllib.parse` | Codificação da mensagem na URL |

## 🚀 Como usar

```bash
pip install openpyxl pyautogui pillow
python app.py
```

1. Crie o arquivo `clientes.xlsx` com as colunas **Nome | Telefone | Vencimento** (a partir da linha 2).
2. Salve um print do botão de enviar do WhatsApp como `seta.png` na mesma pasta.
3. Execute o script e escaneie o QR Code do WhatsApp Web nos primeiros 30 segundos.

## ⚠️ Aviso

Use com responsabilidade e apenas com contatos que autorizaram receber mensagens. Envios em massa podem violar os termos de uso do WhatsApp.

## 📌 Próximos passos

- [ ] Interface gráfica para escolher a planilha
- [ ] Mensagem configurável por arquivo de template
- [ ] Intervalo aleatório entre envios

---
Feito por [Weslei Sousa](https://github.com/joseweslei45-debug)
