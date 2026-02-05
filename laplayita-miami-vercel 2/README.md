# 🏖️ La Playita Miami - Apresentação STR

Pacote completo para deploy da apresentação de investimento no Vercel.

## 📦 Conteúdo do Pacote

```
laplayita-miami-vercel/
├── index.html          → Menu principal com navegação
├── slide-1.html        → Capa (conteúdo pronto)
├── slide-2.html        → Overview (placeholder)
├── slide-3.html        → Performance Financeira (placeholder)
├── slide-4.html        → Análise de Tendências (placeholder)
├── slide-5.html        → Reservas 2026 & Copa (placeholder)
├── slide-6.html        → Despesas Operacionais (placeholder)
├── slide-7.html        → Showcase da Propriedade (placeholder)
├── slide-8.html        → Investment Highlights (placeholder)
├── slide-9.html        → Contato & CTA (placeholder)
├── vercel.json         → Configuração do Vercel
└── README.md           → Este arquivo
```

## 🚀 Deploy no Vercel

### Opção 1: Via GitHub (Recomendado) ⭐

1. **Crie um repositório no GitHub:**
   ```bash
   cd laplayita-miami-vercel
   git init
   git add .
   git commit -m "Initial commit - La Playita presentation"
   git branch -M main
   git remote add origin https://github.com/SEU-USUARIO/laplayita-miami.git
   git push -u origin main
   ```

2. **No Vercel:**
   - Acesse: https://vercel.com/new
   - Clique em "Import Project"
   - Selecione "Import Git Repository"
   - Conecte seu GitHub
   - Selecione o repositório
   - Clique em "Deploy"

3. **Deploy completo em ~1 minuto!** 🎉

### Opção 2: Via Vercel CLI (Mais Rápido)

```bash
# Instalar CLI (se não tiver)
npm i -g vercel

# Na pasta do projeto
cd laplayita-miami-vercel

# Deploy direto
vercel

# Seguir os prompts:
# - Set up and deploy? Yes
# - Which scope? Seu usuário
# - Link to existing project? No
# - Project name? laplayita-miami
# - Directory? ./
# - Override settings? No
```

✅ **Pronto! Link gerado automaticamente**

## 🌐 Personalizar Domínio

Depois do deploy, você pode configurar um domínio personalizado:

### Domínio Vercel (Gratuito):
- Padrão: `random-name-123.vercel.app`
- Personalizado: `laplayita-miami.vercel.app`

**Como configurar:**
1. Acesse seu projeto no Vercel
2. Settings → Domains
3. Add Domain → Digite: `laplayita-miami`
4. Confirme

### Domínio Próprio:
- Exemplo: `invest.laplayitamiami.com`

**Como configurar:**
1. No Vercel: Settings → Domains → Add
2. Digite seu domínio
3. Siga as instruções para configurar DNS
4. Aguarde propagação (~24h)

## ⚠️ IMPORTANTE: Substituir Placeholders

Os arquivos `slide-2.html` até `slide-9.html` contêm **placeholders**.

### Como Adicionar Conteúdo Real:

**Método Manual (Recomendado):**

1. **Exporte cada slide** da apresentação original
2. Copie o HTML completo do slide
3. Abra o arquivo correspondente (ex: `slide-2.html`)
4. Localize a linha com `<div class="slide-content">`
5. **Substitua TODO o conteúdo** entre as tags pelo HTML real
6. Salve o arquivo
7. Faça commit e push (se usando GitHub) ou `vercel --prod`

**Exemplo:**

```html
<!-- ANTES (placeholder) -->
<div class="slide-content">
    <div style="background: ..."">
        ⚠️ Este é um placeholder...
    </div>
</div>

<!-- DEPOIS (conteúdo real) -->
<div class="slide-content">
    <!-- Cole aqui o HTML completo exportado do slide -->
    <div class="financial-slide">
        <h1>Performance Financeira</h1>
        <div class="charts">...</div>
    </div>
</div>
```

## 🎨 Funcionalidades Incluídas

✅ **Navegação Completa:**
- Menu principal (index.html) com grid de 9 slides
- Botões ← → para navegar entre slides
- Botão 🏠 para voltar ao menu
- **Atalhos de teclado:**
  - `←` Slide anterior
  - `→` Próximo slide
  - `Home` ou `Esc` Voltar ao menu

✅ **Design Profissional:**
- Cores navy blue + gold (identidade visual)
- Layout responsivo (desktop/mobile)
- Animações suaves
- Typography elegante

✅ **SEO & Performance:**
- Cache otimizado (vercel.json)
- Rotas configuradas
- Meta tags incluídas

## 📊 Dados da Apresentação

- **Projeção 2026:** $132,830
- **Margem NOI:** 58%
- **Rating:** 4.87★ Superhost 3x
- **Capacidade:** 16 pessoas
- **Quartos:** 4 bedrooms
- **Amenidades:** Heated Pool, Resort-Style Entertainment

## 🔗 Links Úteis

- **Airbnb:** https://airbnb.com/rooms/1330752051728804418
- **Vercel Docs:** https://vercel.com/docs
- **GitHub:** https://github.com

## 💡 Dicas de Uso

### Para Compartilhar com Prospectos:

**Estratégia Dupla:**

1. **Email/WhatsApp (Primeiro Contato):**
   - Envie o PowerPoint como backup
   - Inclua o link Vercel: `laplayita-miami.vercel.app`

2. **Follow-up (Prospectos Sérios):**
   - Envie só o link Vercel
   - Destaque: "Navegue com as setas do teclado!"

**Exemplo de Mensagem:**

```
Olá [Nome],

Segue a apresentação completa da La Playita Miami:

🔗 Apresentação Interativa:
https://laplayita-miami.vercel.app

Destaques:
✅ $132,830 projetados para 2026
✅ Impacto Copa do Mundo (Jun/Jul)
✅ 58% margem NOI
✅ Superhost 3x (4.87★)

Use as setas do teclado para navegar!

À disposição para agendar visita.
```

### Usar Encurtador de Link:

```
bit.ly/laplayita-str
→ redireciona para: laplayita-miami.vercel.app
```

Mais limpo e profissional! 😊

## 🆘 Troubleshooting

### Deploy não funciona?
- Verifique se todos os arquivos .html estão na pasta raiz
- Confirme que vercel.json está presente
- Tente limpar cache: `vercel --prod --force`

### Slides não carregam?
- Verifique se os caminhos estão corretos (slide-1.html, não Slide-1.html)
- Confirme que todos os 9 arquivos existem
- Teste localmente: abra index.html no navegador

### Domínio não resolve?
- Aguarde 24h para propagação DNS
- Verifique configuração no painel Vercel
- Use `nslookup seu-dominio.com` para testar

## 📞 Suporte

Se precisar de ajuda:
1. Consulte a documentação do Vercel
2. Verifique se seguiu todos os passos
3. Teste em ambiente local primeiro

---

**© 2026 La Playita Miami - Premium STR Investment**

🏖️ 65 NW 116th St, Miami, FL 33168
