# João Lucas Almeida

Estudante de **Sistemas de Informação** e técnico de informática. Construo
produtos de ponta a ponta usando IA como alavanca: eu defino o problema, as
regras e o desenho, e oriento agentes de código (Claude Code) a implementar,
testar e documentar.

Os projetos abaixo foram feitos do zero, em poucos dias cada, e estão publicados.

---

## Projetos

### [Portal Duo](https://github.com/joaolucasralmeida/duo-portal-clientes) · portal de clientes para agência de marketing
**[▶ Testar a demonstração](https://joaolucasralmeida.github.io/duo-portal-clientes/)** (dados fictícios)

[![Calendário do Portal Duo](https://raw.githubusercontent.com/joaolucasralmeida/duo-portal-clientes/main/docs/calendario.png)](https://joaolucasralmeida.github.io/duo-portal-clientes/)

Calendário de posts, aprovação de conteúdo com limite de alterações, upload de
vídeo, métricas do Instagram e contratos. Avisa o cliente no WhatsApp quando sai
conteúdo novo.
**4 dias · 63 commits** · React · Supabase (Auth, Storage, RLS, Edge Functions) · WhatsApp Cloud API · Cloudflare

### [Sacra Studio](https://github.com/joaolucasralmeida/sacra-gestao-atelie) · gestão para um ateliê artesanal
Produção, estoque como livro-razão, kits, vendas em lote pós-evento, parcelamento
e cobrança. Regras de dinheiro testadas, permissões por papel no banco.
**~1 semana · 30 testes unitários + 47 verificações de aceitação** · Next.js 16 · TypeScript · Supabase · Vitest

### [Norte](https://github.com/joaolucasralmeida/norte-app) · finanças pessoais no iPhone, com assistente de IA
**[▶ Abrir o app](https://joaolucasralmeida.github.io/norte-app/)**

App instalável (PWA) que funciona offline e sincroniza entre aparelhos. O
**[assistente de IA](https://github.com/joaolucasralmeida/norte-app/tree/main/gemini-worker)**
é um agente na **API do Gemini**, sem SDK: pesquisa o preço na web, cita as fontes
e propõe a meta de compra para o usuário confirmar.
- Loop de *function calling* com 3 ferramentas, resposta em streaming (SSE)
- Troca automática de modelo quando um está lotado (`503`), sem queimar cota no `429`
- Prompt com regras verificáveis e defesa contra injeção de prompt vinda das páginas lidas
- 10 testes automáticos que simulam as APIs do Gemini e da Tavily

JavaScript puro · Supabase · Gemini API (function calling) · Tavily · Cloudflare Workers

### No trabalho · controle de estoque e patrimônio da TI
Sistema interno da manutenção de TI onde trabalho: catálogo, bens patrimoniados,
ordem de serviço, termo de entrega e manutenção preventiva, com integração ao GLPI
para abrir chamados. Node.js sem dependências (a rede é fechada), 71 rotas,
18 tabelas e 12 verificações automáticas. Em migração para Oracle.
*Código interno, não publicado.*

---

## Como eu trabalho com IA

- **Contexto antes de código.** Cada projeto tem um `CLAUDE.md` que diz ao agente
  quem é o usuário, quais regras não se negociam e o que nunca fazer com dados reais.
- **Regras críticas no banco.** Permissão e regra de negócio ficam em RLS, trigger
  e função SQL, não só na tela. Assim o que a IA gera no front não fura o sistema.
- **Testes como rede de segurança.** Domínio em funções puras e testadas, para
  pedir mudanças ao agente e verificar que nada quebrou.
- **Commits pequenos e legíveis**, para revisar e desfazer cada passo.

## Formação e estudos

- **Sistemas de Informação**: Multivix (em andamento; antes no Ifes, 2023–2025)
- **Santander Coders 2023.2**: trilha Back-end
- **Estudando agora** (meta: janeiro de 2027):
  - .NET: API completa com DDD, SOLID, testes, Docker, Azure DevOps e deploy no Azure (60h)
  - Angular (154h), com o plano de consumir a API do curso de .NET num projeto full-stack
- C# para iniciantes (Udemy) · HTML e CSS3 (Curso em Vídeo) · Latinoware 2023

## Ferramentas

Claude Code · Gemini API · Supabase · Node.js · React · Next.js · TypeScript · SQL · PostgreSQL · Oracle · GLPI · Git · Cloudflare · C#/.NET e Angular (estudando)

[LinkedIn](https://www.linkedin.com/in/jo%C3%A3o-lucas-almeida-058751263/)
