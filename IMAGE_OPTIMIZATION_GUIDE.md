# 📸 GUIA DE OTIMIZAÇÃO DE IMAGENS PARA SEO

## 🎯 Por que Otimizar Imagens para SEO?

1. **Ranking em Busca de Imagens**: Aparece em google.com/images
2. **Performance**: Melhor velocidade = melhor ranking geral
3. **User Experience**: Carregamento mais rápido = menos bounce
4. **Schema.org**: Google reconhece e exibe imagens em rich snippets

## 🔧 Como Otimizar Alt Text

### ✅ BOM Alt Text
```html
<!-- Descritivo e relevante para SEO -->
<img src="caminhao-munck.jpg" 
     alt="Caminhão Munck de 35 a 45 toneladas para locação - Top Locações Nordeste"
     loading="lazy">
```

### ❌ RUIM Alt Text
```html
<!-- Vago e sem contexto -->
<img src="image1.jpg" alt="foto">
<img src="caminhao.jpg" alt="imagem">
```

## 📋 Checklist: Melhorias de Imagens a Fazer

### NAVEGAÇÃO (Header)
- [ ] `logo.png` → Alt: "Top Locações & Serviços - Logo da Empresa de Locação"

### HERO SECTION
- [ ] Hero video → Descrição clara
- [ ] Imagens de fundo → Alt tags apropriadas

### SEÇÃO SOBRE
- [ ] Imagem da frota → Alt: "Frota de Caminhões e Equipamentos Pesados da Top Locações em ação"

### SEÇÃO FROTA (Gallery)
Adicionar `loading="lazy"` a todas:
- [ ] Caminhão Munck → "Caminhão Munck de 35 a 45 toneladas para movimentação de cargas pesadas"
- [ ] Caminhão Pipa → "Caminhão Pipa de 10.000L a 20.000L para combate a poeira e irrigação"
- [ ] Escavadeira → "Escavadeiras Hidráulicas para escavação profunda em obras"
- [ ] Caminhão Basculante → "Caminhão basculante 6m³, 12m³ e 20m³ para transporte de materiais"
- [ ] Caminhão Prancha → "Caminhão prancha para transporte de máquinas pesadas e cargas especiais"
- [ ] Pá Carregadeira → "Pá Carregadeira para carregamento de materiais e movimentação"

### SEÇÃO EQUIPAMENTOS
Cada card de equipamento deve ter:
- [ ] Alt text descritivo com especificações técnicas
- [ ] `loading="lazy"` (abaixo da dobra)
- [ ] Imagem otimizada em tamanho

### SEÇÃO CLIENTES
- [ ] Todas as logos → Alt: "Logo de [Nome da Empresa] - Cliente da Top Locações"

### FOOTER
- [ ] Logo → Alt: "Top Locações & Serviços Footer Logo"

## 🖼️ Otimização de Tamanho de Arquivo

### Formatos Recomendados:
1. **Produtos/Equipamentos**: WebP (melhor compressão) + JPEG fallback
2. **Logos**: PNG (transparência)
3. **Ícones**: SVG (escalável)
4. **Hero Image**: JPEG otimizado (80-85% qualidade)

### Código Melhorado com Picture Element:
```html
<picture>
  <source srcset="imagem.webp" type="image/webp">
  <source srcset="imagem.jpg" type="image/jpeg">
  <img src="imagem.jpg" 
       alt="Descrição completa da imagem para SEO"
       loading="lazy"
       width="600" 
       height="400">
</picture>
```

## ⚡ Tamanhos Recomendados

| Tipo | Largura | Altura | Peso Máximo |
|------|---------|--------|------------|
| Logo | 200-400 | 80-160 | 100 KB |
| Card Imagem | 600 | 400 | 150 KB |
| Hero Banner | 1920 | 1080 | 400 KB |
| Thumbnail | 300 | 300 | 80 KB |
| Ícone | 100 | 100 | 20 KB |

## 🔍 Testando Otimizações

### Google Page Speed Insights
https://pagespeed.web.dev
- Ingira a URL
- Veja recomendações específicas
- Monitore Core Web Vitals

### Rich Results Test (Rich Snippets)
https://search.google.com/test/rich-results
- Cole o código HTML
- Veja se Schema.org está sendo reconhecido

### Lighthouse
Ferramentas → DevTools → Lighthouse
- Rode um teste
- Veja pontuação de Performance
- Corrija problemas

## 📊 Schema.org para Imagens

Adicionar na imagem de produtos/equipamentos:
```html
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "ImageObject",
  "name": "Caminhão Munck",
  "url": "https://example.com/caminhao-munck.jpg",
  "description": "Caminhão Munck de 35 a 45 toneladas para movimentação de cargas pesadas",
  "thumbnailUrl": "https://example.com/thumbs/caminhao-munck.jpg"
}
</script>
```

## 🚀 Próximas Ações

1. **Fase 1**: Adicionar `loading="lazy"` em todas as imagens abaixo da dobra
2. **Fase 2**: Melhorar todos os alt texts
3. **Fase 3**: Converter imagens principais para WebP
4. **Fase 4**: Adicionar Schema.org ImageObject para produtos
5. **Fase 5**: Monitorar em Google Images Search

---

**Impacto Esperado**:
- ⬆️ 30-40% de melhoria em Page Speed
- ⬆️ 25-35% em tráfego de Google Images
- ⬆️ 10-15% em ranking geral
