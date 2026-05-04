# Gôbra — Landing Pages v1.0

Sistema de 4 landing pages independentes para a Gôbra.

## Arquitetura

```
gobra.ai/                    → index.html       (institucional)
gobra.ai/clientes            → clientes.html    (para quem contrata)
gobra.ai/prestadores         → prestadores.html (para quem executa)
gobra.ai/parceiros           → parceiros.html   (para instituições financeiras)
```

## Estratégia de conteúdo

### Institucional
Vitrine de marca curta. Apresenta a plataforma e roteia o visitante para a landing certa por persona.
- **Hook:** "A obra que você controla."
- **Punch line dark:** "Três agentes. Três dores. Uma causa raiz."
- **CTA:** Quero saber mais

### Clientes
Tom emocional, próximo. Vocabulário do dia-a-dia, sem jargão financeiro.
- **Hook:** "Pague apenas pelo que for entregue."
- **Argumentos:** custódia, score do prestador, reembolso automático, app
- **Punch line dark:** "Quatro proteções blindadas em todas as obras."

### Prestadores
Tom operacional, parceria, prático.
- **Hook:** "Capital de giro na hora e clientes que pagam de verdade."
- **Argumentos:** crédito barato, pagamento garantido, demanda qualificada, histórico
- **Punch line dark:** "De obra em obra, você cresce."

### Parceiros financeiros
Tom técnico-financeiro. Vocabulário do setor: LTV, NPL, originação, colateral.
- **Hook:** "Originação qualificada com colateral líquido."
- **Argumentos:** colateral líquido, score multifonte, ciclo curto, API
- **Punch line dark:** "Crédito que se autoavalia. Risco que se autodefende."

## Filosofia visual

**Leveza como padrão, peso como exceção.**
- Background branco/snow domina (8+ seções por landing)
- Inversão dark estratégica em 2 momentos por landing:
  1. Síntese narrativa (pausa para absorção)
  2. CTA final (chamada à ação)

## CTA universal

Todas as landings usam **"Quero saber mais"** como CTA universal, abrindo um modal de contato com formulário simples (nome, email, telefone, persona, mensagem). Submit é placeholder por enquanto — quando o backend estiver pronto, plugar lá.

## Tecnologia

- HTML5 + CSS3 puro (sem frameworks)
- Tipografia: Inter via Google Fonts CDN (fallback: system-ui)
- Vanilla JavaScript para animações de scroll, modal, FAQ
- Responsive mobile-first
- Zero dependências externas além do Google Fonts

## Deploy

Cada arquivo HTML é standalone e pode ser hospedado em qualquer plataforma:
- Vercel / Netlify / GitHub Pages: arrastar e soltar
- Cloudflare Pages: conectar repositório
- Servidor próprio: copiar para o webroot

## Customização

Tokens de design no `:root` de cada arquivo:
- `--brand: #CCFCCB` (verde pastel)
- `--algae: #96E6B3`
- `--spring: #568259` (CTAs)
- `--deep: #2C5430`
- `--ink: #1A1A1A`

## Versão

v1.0 · Maio 2026
