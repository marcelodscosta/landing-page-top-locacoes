# GOOGLE SEARCH CONSOLE VERIFICATION GUIDE

## 🔐 Passo 1: Acessar Google Search Console

1. Abra: https://search.google.com/search-console
2. Clique em "Adicionar propriedade"
3. Escolha o tipo de propriedade: **Domínio**
4. Insira: `topgruposervicos.com` (isso indexará todo o domínio)

## ✅ Passo 2: Verificar a Propriedade

### Opção A: Registro DNS (RECOMENDADO)
1. Na GSC, copie o token TXT gerado
2. Acesse seu painel de controle do domínio (registrador/hospedagem)
3. Vá para gerenciar registros DNS
4. Adicione um novo registro TXT:
   - **Nome**: `@` (ou deixe em branco)
   - **Valor**: Cole o token fornecido pela GSC
   - **TTL**: 3600 (ou padrão)
5. Clique em "Verificar"

### Opção B: Meta tag HTML
Se não tiver acesso ao DNS:
1. Copie a meta tag fornecida pela GSC
2. Adicione no `<head>` do index.html após as outras meta tags:
```html
<meta name="google-site-verification" content="COPIE_AQUI_O_CODIGO" />
```

### Opção C: Upload de arquivo
1. Download do arquivo HTML da GSC
2. Faça upload na raiz do servidor (public_html/)

## 📝 Passo 3: Submeter o Sitemap

1. Na GSC, no menu lateral, clique em **Sitemaps**
2. Digite na caixa de texto: `sitemap.xml`
3. Clique em "Enviar"

## 🔍 Passo 4: Verificar Indexação

Após 24-48 horas:
1. Vá para **Cobertura** na GSC
2. Verá quantas páginas foram indexadas
3. Se houver erros, clique neles para corrigir

## 🛠️ Passo 5: Monitorar SEO

No painel da GSC você verá:
- **Performance**: Cliques, impressões, CTR, posição
- **Cobertura**: Problemas de indexação
- **Experiência**: Core Web Vitals
- **Melhorias**: Dados estruturados reconhecidos

## 📊 Ferramentas Complementares

### Google Analytics 4 (GA4)
Para monitorar comportamento dos visitantes:
1. Acesse: https://analytics.google.com
2. Crie nova propriedade: `www.topgruposervicos.com`
3. Copie o Google Tag (G-XXXXXXXX)
4. Adicione no `<head>` do index.html:
```html
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXX');
</script>
```

### Google My Business (GMB)
Para aparecer em buscas locais:
1. Acesse: https://www.google.com/business
2. Crie/edite a listagem do negócio
3. Adicione:
   - Endereço completo
   - Telefone
   - Website
   - Horário de funcionamento
   - Fotos
   - Descrição detalhada

### Bing Webmaster Tools
1. Acesse: https://www.bing.com/webmasters
2. Adicione o site
3. Envie o sitemap

## 🚀 Dicas Finais para Melhor SEO

1. **Conteúdo**: Mantenha o site atualizado com blog posts
2. **Backlinks**: Procure por parceria com sites relevantes
3. **Velocidade**: Optimize imagens e use CDN
4. **Mobile**: Sempre teste em celulares
5. **Experiência**: Melhore o layout e usabilidade
6. **Keywords**: Pesquise palavras-chave locais e regionais

## 📈 Métricas Esperadas

Após 3-6 meses com bom SEO:
- Aumento de 200-400% em impressões
- Aumento de 150-300% em cliques
- Melhora na posição média (top 10)
- Diminuição do bounce rate

---

**Criado em**: 5 de abril de 2026
**Status**: Guia Completo
