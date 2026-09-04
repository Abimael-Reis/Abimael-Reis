
<!-- ================= COMEÇA O README ================= -->

# Olá, eu sou o Abimael 👋

Desenvolvedor de sistemas. Gosto de resolver problema real de operação: sistemas
internos, automações e integrações que rodam todo dia em produção, de ERP e
atendimento por WhatsApp a PDV, PIX e leitura de NF-e.

## 🚀 Tecnologias

- **Back-end:** Python (FastAPI, Flask), Node.js (Express), SQLAlchemy, Alembic
- **Front-end:** React, Next.js, TypeScript, Tailwind CSS, HTML/CSS
- **Mobile:** React Native (Expo), Android (Java/Kotlin), Flutter
- **Dados:** PostgreSQL, SQLite, SQL Server, Pandas, openpyxl
- **Infra:** Docker / Docker Compose, Nginx, Cloudflare Tunnel, Linux, PM2
- **Automação & IA:** Playwright, Selenium, faster-whisper (transcrição), LLMs em fluxos internos
- **Integrações:** WhatsApp (Baileys), PIX/Sicredi, PagSeguro, iFood, NF-e/SEFAZ, Bluesoft Cosmos, Google Meet

## 📌 Projetos em destaque

- **Monitor de Rede** — Painel em Docker
  (FastAPI + SQLite) que mapeia todos os dispositivos da rede local, detecta aparelhos
  novos e guarda histórico de conexão. Como o Docker Desktop no Windows nunca enxerga a
  placa de rede física, a varredura roda num agente nativo (ping sweep + tabela ARP) que
  entrega o resultado ao container via API — o README documenta as duas alternativas
  testadas e por que nenhuma funcionou.
- **DiskAB — Gestão para Distribuidora de Bebidas** —
  Sistema full-stack containerizado (FastAPI + PostgreSQL + React/Nginx) com produtos,
  estoque, PDV, pedidos e relatórios. Cadastro por leitura de código de barras consultando
  a API Bluesoft Cosmos (EAN → nome, NCM, CEST, peso, imagens) e integração com o iFood
  via OAuth2 + webhook de pedidos.
- **Ecommerce** — Loja em Next.js 16 +
  React 19 + Tailwind 4 com catálogo público, carrinho e checkout que dispara o resumo do
  pedido direto no WhatsApp da loja, além de painel admin para produtos e pedidos. Sobe em
  Docker com volumes persistentes e vai ao ar por Cloudflare Tunnel, sem IP fixo.
- **Cadastro de Produtos (NF-e + Cosmos)** —
  CLI em Python que lê XMLs de NF-e/NFC-e, consulta cada EAN na API Cosmos e devolve uma
  planilha `.xlsx` pronta para o cadastro, com uma aba já no formato do formulário do
  sistema e outra com todos os dados brutos para conferência. Transformou um cadastro
  manual e demorado em um comando só.
- **SMS Gateway Android** — App Android que
  virou *cliente* em vez de servidor: faz polling na API a cada X segundos, busca as
  mensagens pendentes, envia os SMS pelo chip e devolve o status. Assim o celular manda
  SMS a partir do sistema web sem precisar de IP fixo nem porta aberta.

## 💼 Experiência (código proprietário, sem repositório público)

Sistemas que desenvolvi e mantenho na empresa em que trabalho:

- **Plataforma de atendimento por WhatsApp** — Node.js + Baileys com múltiplas instâncias
  (vários números), painel administrativo, controle de acesso por instância, métricas de
  SLA e sincronização de ~12 mil contatos vindos do ERP.
- **Assistente em linguagem natural para o ERP** — LLM sobre os protocolos do sistema:
  responde em português a perguntas como "eventos em aberto que eu já respondi", lê todo o
  histórico do chamado e chega a redigir a resposta — que só é publicada após revisão humana.
- **Bot gravador de reuniões** — entra no Google Meet via Playwright em display virtual
  (Xvfb + PulseAudio), grava em MP4 com ffmpeg, transcreve localmente com faster-whisper e
  devolve resumo automático. Isola display, sink de áudio e perfil por sala, gravando
  várias reuniões em paralelo.
- **CRM / B.I. comercial** — FastAPI que lê o ERP legado em modo somente-leitura e mantém
  base própria: clientes ativos por janela de compra, contatos por CNPJ e ciclo de compra
  por produto, princípio ativo, grupo e fabricante.
- **App mobile interno** — React Native + Expo (navegação, câmera, offline com AsyncStorage, Zustand).
- **Integrações com Sicredi** — cobranças, conciliação de liquidações e webhooks.

## 🌱 Atualmente aprendendo

- Arquitetura de bancos de dados
- React-Native

## 📫 Contato

- E-mail: alexabimaelreis@gmail.com

<!-- ================= TERMINA O README ================= -->
