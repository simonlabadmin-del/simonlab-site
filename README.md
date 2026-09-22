# SimonLab — Landing Page

Landing page institucional da SimonLab. Site **estático** (HTML + CSS inline + imagens). Sem build, sem framework, sem dependências — abre em qualquer lugar.

## Estrutura
```
index.html          → a página inteira (HTML + CSS + JS inline)
assets/
  logo.png              → logo SIMONLAB (usado no topo e no rodapé)
  hero-datacenter.jpg   → imagem de fundo do topo (hero)
  problema-mapa.jpg     → seção "O Problema"
  diagnostico-laptop.jpg→ seção "Diagnóstico"
  predio-simonlab.jpg   → imagem do CTA final (rodapé)
```

## Rodar localmente
Abra o `index.html` no navegador (duplo clique) — ou, pra servir:
```bash
npx http-server . -p 8080
```

## Publicar (escolha um)
- **Vercel** (grátis): crie conta em vercel.com → New Project → arraste esta pasta (ou conecte um repositório). Deploy automático com HTTPS.
- **Netlify** (grátis): netlify.com → arraste a pasta na área de deploy. Pronto.
- **GitHub Pages / Cloudflare Pages**: suba a pasta num repositório e ative o Pages.
- **Servidor próprio (Apache/Nginx)**: copie os arquivos pra raiz do site.

**Domínio SimonLab:** depois de publicar, aponte o domínio no painel do host (em geral: adicionar o domínio no projeto + criar os registros DNS que o host indicar). HTTPS costuma ser automático.

## Editar
Tudo está no `index.html`. Para trocar textos, procure a seção e edite direto. Para trocar imagens, substitua o arquivo em `assets/` mantendo o mesmo nome (ou ajuste o `src` no HTML).

## ⚠️ Pontos de atenção (ajustar antes de divulgar)
1. **`assets/diagnostico-laptop.jpg`** — a tela do laptop tem escrito **"SIMONTECH"** (nome antigo). Trocar por uma imagem com "SIMONLAB" ou sem nome. Aparece na seção "Diagnóstico".
2. **WhatsApp** — o número configurado é **+55 11 96566-9781**. Confira se é o número final (aparece em 3 lugares: botão do topo, CTA final e botão flutuante). Busque por `wa.me/5511965669781` no HTML.
3. **Instagram / contatos** — atualize se houver links a acrescentar.
4. **Fontes** — carregadas via Google Fonts (Inter), precisa de internet. Se quiser 100% offline, baixe a fonte e referencie localmente.

Qualquer dúvida, o Dr. Marcos tem o contato de quem montou. 🚀
