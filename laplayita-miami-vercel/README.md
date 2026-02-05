# 🏠 La Playita Miami - Apresentação para Vercel

Pacote completo para deploy da apresentação interativa **La Playita Miami STR Investment** no Vercel.

## 📦 Conteúdo do Pacote

```
laplayita-miami-vercel/
├── index.html          # Página inicial com menu de navegação
├── slide-1.html        # Slide 1: Capa
├── slide-2.html        # Slide 2: Overview
├── slide-3.html        # Slide 3: Performance Financeira
├── slide-4.html        # Slide 4: Análise de Tendências
├── slide-5.html        # Slide 5: Reservas 2026 & Copa do Mundo
├── slide-6.html        # Slide 6: Despesas Operacionais
├── slide-7.html        # Slide 7: Showcase da Propriedade
├── slide-8.html        # Slide 8: Destaques do Investimento
├── slide-9.html        # Slide 9: Contato & Próximos Passos
├── vercel.json         # Configuração do Vercel
└── README.md           # Este arquivo
```

## 🚀 Deploy no Vercel (3 Métodos)

### **Método 1: Interface Web (Mais Fácil) ⭐ RECOMENDADO**

1. **Acesse:** https://vercel.com/new
2. **Arraste a pasta** `laplayita-miami-vercel` para a área de upload
3. **Configure o projeto:**
   - Project Name: `laplayita-miami` (ou outro nome)
   - Framework Preset: `Other` (deixar em "Other")
   - Root Directory: `./` (raiz do projeto)
4. **Clique em "Deploy"**
5. **Aguarde 30-60 segundos** ⏳
6. **Pronto!** Seu link estará disponível: `laplayita-miami.vercel.app`

### **Método 2: Via CLI (Para Desenvolvedores)**

```bash
# 1. Instalar Vercel CLI (se ainda não tiver)
npm install -g vercel

# 2. Login no Vercel
vercel login

# 3. Navegar até a pasta do projeto
cd laplayita-miami-vercel

# 4. Deploy
vercel

# 5. Para deploy em produção
vercel --prod
```

### **Método 3: GitHub + Vercel (Deploy Automático)**

1. **Criar repositório no GitHub:**
   - Faça upload da pasta para um repositório GitHub

2. **Conectar ao Vercel:**
   - Acesse https://vercel.com/new
   - Clique em "Import Git Repository"
   - Selecione seu repositório
   - Configure e deploy

3. **Vantagem:** Cada push no GitHub faz deploy automático! 🔄

## 🎨 Personalizar Domínio

### **Domínio Gratuito (.vercel.app)**
Após o deploy, você terá automaticamente:
- `laplayita-miami.vercel.app` (ou o nome que escolher)

### **Domínio Personalizado (Próprio)**

1. **No dashboard do Vercel:**
   - Vá em "Settings" → "Domains"
   - Clique em "Add Domain"
   - Digite seu domínio: `invest.laplayitamiami.com`

2. **Configure DNS:**
   - Adicione um registro CNAME no seu provedor de domínio
   - Aponte para: `cname.vercel-dns.com`

3. **Aguarde propagação** (5-30 minutos)

4. **Exemplos de domínios:**
   - `invest.laplayitamiami.com`
   - `presentation.laplayitamiami.com`
   - `opportunity.laplayitamiami.com`

## ⚠️ IMPORTANTE: Conteúdo dos Slides

Os arquivos `slide-1.html` até `slide-9.html` estão com **conteúdo placeholder**.

### **Como Substituir pelo Conteúdo Real:**

1. **Exporte os slides do sistema Genspark:**
   - No sistema de slides, use a ferramenta de export
   - Copie o HTML completo de cada slide

2. **Substitua o conteúdo:**
   - Abra cada arquivo `slide-X.html` em um editor de texto
   - Localize a seção `<div class="slide-content">`
   - **Substitua APENAS o conteúdo interno** desta div
   - **NÃO APAGUE** a navegação (nav-bar) no topo

3. **Estrutura correta:**
   ```html
   <div class="slide-content">
       <!-- COLE SEU CONTEÚDO AQUI -->
       <!-- Todo o HTML do slide exportado -->
   </div>
   ```

4. **Faça isso para todos os 9 slides**

5. **Re-deploy:**
   - Se usou interface web: arraste a pasta novamente
   - Se usou CLI: execute `vercel --prod`
   - Se usou GitHub: apenas faça commit e push

## ✨ Funcionalidades Incluídas

### **Navegação Intuitiva:**
- ✅ Menu inicial com cards dos 9 slides
- ✅ Botões "Anterior" e "Próximo" em cada slide
- ✅ Botão "Menu" para voltar ao índice
- ✅ Contador de slides (X / 9)

### **Navegação por Teclado:**
- ⬅️ **Seta Esquerda:** Slide anterior
- ➡️ **Seta Direita:** Próximo slide
- **ESC:** Voltar ao menu principal

### **Design Responsivo:**
- 📱 Mobile-friendly
- 💻 Desktop otimizado
- 🎨 Design premium com cores navy blue e gold

## 🔧 Configurações Avançadas

### **Cache Control**
O `vercel.json` já está configurado com cache de 1 hora para melhor performance.

### **Adicionar Analytics**

Para rastrear visualizações, adicione Google Analytics no `index.html`:

```html
<!-- Antes do </head> -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXXXX');
</script>
```

### **Senha de Acesso (Opcional)**

Para proteger a apresentação com senha:

1. **Adicione Vercel Password Protection:**
   - No dashboard do Vercel: Settings → General
   - Ative "Password Protection"
   - Defina uma senha
   - Apenas pessoas com a senha podem acessar

## 📊 Dados Atualizados na Apresentação

- **Receita Projetada 2026:** $132,830
- **NOI Margem:** 58%
- **Superhost:** 3x consecutivo
- **Rating:** 4.87 ⭐
- **Capacidade:** 16 pessoas
- **Quartos:** 4 bedrooms
- **Impacto Copa do Mundo:** Junho e Julho 2026

## 🎯 Como Usar com Prospectos

### **1. Envio por Email/WhatsApp:**

```
Olá [Nome],

Segue a apresentação completa da La Playita Miami:

🔗 Link Interativo: https://laplayita-miami.vercel.app

Destaques:
✅ $132,830 projetados para 2026
✅ 58% margem NOI
✅ Impacto Copa do Mundo 2026
✅ Superhost 3x (4.87⭐)

Use as setas ← → para navegar ou clique no menu.

Disponível para visita e perguntas!
```

### **2. Encurtar o Link (Opcional):**

Use **bit.ly** ou **tinyurl.com** para criar:
- `bit.ly/laplayita-miami`
- `tinyurl.com/laplayita-str`

Fica mais limpo e profissional! 🎯

## 🆘 Suporte e Troubleshooting

### **Deploy falhou?**
- ✅ Verifique se todos os arquivos HTML estão válidos
- ✅ Verifique se o `vercel.json` está na raiz
- ✅ Tente fazer deploy novamente

### **Imagens não aparecem?**
- ✅ Certifique-se que as imagens estão em URLs públicas ou base64
- ✅ Se usar URLs, verifique se são acessíveis sem autenticação

### **Gráficos não funcionam?**
- ✅ Certifique-se que o Chart.js está incluído no HTML
- ✅ Verifique se os scripts estão dentro do HTML do slide

### **Navegação quebrada?**
- ✅ NÃO apague a `<nav class="nav-bar">` ao substituir conteúdo
- ✅ Mantenha apenas a div `<div class="slide-content">` com seu conteúdo

## 📝 Logs de Deploy

Após o deploy, você pode ver logs em:
- **Interface Web:** https://vercel.com/dashboard → Seu Projeto → "Deployments"
- **CLI:** `vercel logs`

## 🎉 Pronto para Usar!

Após seguir estes passos, você terá:
- ✅ Apresentação online com domínio personalizado
- ✅ Navegação intuitiva com teclado e botões
- ✅ Design responsivo e profissional
- ✅ Performance otimizada com cache
- ✅ Pronto para compartilhar com prospectos!

---

## 📞 Contatos

**Propriedade:** La Playita Miami  
**Endereço:** 65 NW 116th St, Miami, FL 33168  
**Airbnb:** https://airbnb.com/rooms/1330752051728804418  

**Deploy Date:** Fevereiro 2026  
**Versão:** 1.0  

---

💡 **Dica Final:** Teste a apresentação em diferentes dispositivos (mobile, tablet, desktop) antes de enviar para prospectos. Use as ferramentas de desenvolvedor do Chrome (F12) para testar responsividade.

🚀 **Bom deploy e boas vendas!**
