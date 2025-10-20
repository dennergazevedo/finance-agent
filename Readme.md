# 🤖 Agente Financeiro via WhatsApp — N8N + WAHA

Este projeto implementa um **Agente Financeiro Inteligente** integrado ao **WhatsApp**, utilizando **N8N**, **WAHA** e **Google Sheets**.  
O agente é capaz de **gerir suas finanças**, e salvar relatórios em tempo real via WhatsApp.

> 🎥 **Assista ao tutorial completo no YouTube:**  
> [https://youtu.be/7vlcbM84ZM0](https://youtu.be/7vlcbM84ZM0)

---

## 🚀 Tecnologias Utilizadas

- [**N8N**](https://n8n.io/) — Plataforma de automação de fluxos de trabalho.
- [**WAHA (WhatsApp HTTP API)**](https://waha.devlike.pro/) — Conector para WhatsApp.
- [**Docker**](https://www.docker.com/) — Containerização para fácil execução em diferentes sistemas operacionais.
- **Node.js**, **JavaScript**, **JSON**, **APIs REST**.
- [**Sheets**](https://sheets.new/) — Planilha do Google para controle.

---

## 🧩 Estrutura do Repositório

```bash
├── docker/
│   ├── arm/
│   │   └── docker-compose.yml
│   ├── linux/
│   │   └── docker-compose.yml
│   └── windows/
│       └── docker-compose.yml
│
├── workflows/
│   └── agente-financeiro.json  # Workflow N8N exportado
│
└── README.md
```

Cada pasta dentro de `docker` contém um `docker-compose.yml` configurado para o respectivo sistema operacional:

**arm** → dispositivos ARM (como Raspberry Pi ou Apple M* Series)

**linux** → distribuições Linux

**windows** → ambiente Windows

## ⚙️ Como Executar
1. Clone este repositório
```bash
git clone https://github.com/<seu-usuario>/<nome-do-repositorio>.git
cd <nome-do-repositorio>
```

2. Escolha o ambiente
Entre na pasta correspondente ao seu sistema operacional:
```bash
cd docker/arm     # ou docker/linux / docker/windows
```

3. Suba os containers com Docker Compose
```bash
docker-compose up -d
```

Isso iniciará:
- O servidor N8N
- O conector WAHA
- Todas as dependências necessárias para o agente

## 💬 Configuração do WAHA (WhatsApp)
Acesse a documentação oficial no site do [WAHA](https://waha.devlike.pro/docs/overview/introduction/)

## 🧠 Importando o Workflow no N8N
Acesse a documentação oficial no site do [N8N](https://docs.n8n.io/courses/level-one/chapter-6/)

## 🧑‍💻 Autor
Denner Azevedo
Tech Lead & Senior Engineer @ Cia. Hering
💼 Focado em performance, automação, IA aplicada e integrações inteligentes
📺 [YouTube](https://www.youtube.com/@devdenegociosmg)

## 🪪 Licença
Este projeto está sob a licença MIT — sinta-se livre para usar, modificar e compartilhar.