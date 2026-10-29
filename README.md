# João Lucas Almeida

Estudante de **Sistemas de Informação** e técnico de informática. Construo
produtos de ponta a ponta usando IA como alavanca: eu defino o problema, as
regras e o desenho, e oriento agentes de código (Claude Code) a implementar,
testar e documentar.

Os projetos abaixo foram feitos do zero, em dias, e estão publicados e em uso.

---

## Projetos

### [Portal Duo](https://github.com/joaolucasralmeida/duo-portal-clientes) · portal de clientes para agência de marketing
Calendário de posts, aprovação de conteúdo com limite de alterações, upload de
vídeo, métricas do Instagram e contratos. Avisa o cliente no WhatsApp quando sai
conteúdo novo.
**4 dias · 63 commits** · React · Supabase (Auth, Storage, RLS, Edge Functions) · WhatsApp Cloud API · Cloudflare

### [Sacra Studio](https://github.com/joaolucasralmeida/sacra-gestao-atelie) · gestão para um ateliê artesanal
Produção, estoque como livro-razão, kits, vendas em lote pós-evento, parcelamento
e cobrança. Regras de dinheiro testadas, permissões por papel no banco.
**~1 semana · 30 testes unitários + 47 verificações de aceitação** · Next.js 16 · TypeScript · Supabase · Vitest

### [Norte](https://github.com/joaolucasralmeida/norte-app) · finanças pessoais no iPhone, com assistente de IA
App instalável (PWA) que funciona offline, sincroniza entre aparelhos e tem um
chat com **Gemini** que pesquisa preços na web por chamada de ferramentas, com
tratamento do que o modelo devolve como conteúdo não confiável.
JavaScript puro · Supabase · Gemini (tool calling) · Tavily · Cloudflare Workers

---

## Como eu trabalho com IA

- **Contexto antes de código.** Cada projeto tem um `CLAUDE.md` que diz ao agente
  quem é o usuário, quais regras não se negociam e o que nunca fazer com dados reais.
- **Regras críticas no banco.** Permissão e regra de negócio ficam em RLS, trigger
  e função SQL, não só na tela. Assim o que a IA gera no front não fura o sistema.
- **Testes como rede de segurança.** Domínio em funções puras e testadas, para
  pedir mudanças ao agente e verificar que nada quebrou.
- **Commits pequenos e legíveis**, para revisar e desfazer cada passo.

## Ferramentas

Claude Code · Gemini API · Supabase · React · Next.js · TypeScript · SQL/PostgreSQL · Oracle · C#/.NET (estudando) · Cloudflare
