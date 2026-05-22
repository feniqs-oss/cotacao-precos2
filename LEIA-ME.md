# 🛒 Cotação de Preços — PWA

App para consulta de preços em supermercados de São Sebastião/SP.
Consulta: Pão de Açúcar, Shibata e Semar.

---

## 📦 Arquivos

```
cotacao-pwa/
├── index.html       ← App principal
├── manifest.json    ← Config do PWA
├── sw.js            ← Service Worker
└── icons/
    ├── icon-192.png
    └── icon-512.png
```

---

## 🚀 Como hospedar (grátis) e instalar no celular

### Opção 1 — Netlify Drop (mais fácil, 2 minutos)

1. Acesse https://app.netlify.com/drop
2. Arraste a pasta `cotacao-pwa` inteira para a área indicada
3. Netlify gera um link HTTPS automático (ex: `https://abc123.netlify.app`)
4. No celular Android, abra esse link no Chrome
5. Chrome mostra banner "Adicionar à tela inicial" → toque para instalar

### Opção 2 — GitHub Pages

1. Crie repositório no GitHub
2. Envie os arquivos
3. Ative GitHub Pages em Settings → Pages → branch main
4. Acesse o link gerado no celular

### Opção 3 — Servidor local (para testes)

```bash
cd cotacao-pwa
python3 -m http.server 8080
# Acesse http://localhost:8080 no navegador
```

---

## 🔑 Chave de API

Na primeira abertura do app, informe sua chave da Anthropic API:
- Obtenha em: https://console.anthropic.com/keys
- A chave fica salva apenas no dispositivo (localStorage)
- Formato: `sk-ant-api03-...`

---

## 📱 Como instalar no Android

1. Abra o link do app no **Chrome**
2. Toque nos 3 pontinhos (⋮) no canto superior direito
3. Toque em **"Adicionar à tela inicial"**
4. Confirme → o app aparece como ícone na tela inicial

---

## ✅ Funcionalidades

- Busca em tempo real nos 3 supermercados via IA
- Resultados ordenados por menor preço (até 7 por mercado)
- Links diretos para cada produto nos sites
- Seta piscando → clique para ir ao produto
- Promoções destacadas em vermelho com link específico
- Tabela de variações (tamanhos, sabores, marcas)
- Nova consulta limpa o histórico
- Funciona como app nativo no Android
