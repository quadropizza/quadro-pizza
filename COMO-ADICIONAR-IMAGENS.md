# 📸 Como adicionar as imagens dos produtos

Você precisa salvar cada foto dentro da pasta certa, com o nome certo.
Quando salvar, o site já aparece com elas (recarregue com Ctrl+F5).

## 📂 Onde está a pasta?

`c:\Users\HP\OneDrive\Área de Trabalho\Quadrô pizza\images\`

Dentro tem 3 subpastas:
- `images/pizzas/` — pizzas 25cm
- `images/mini/` — pizzas mini
- `images/combos/` — banners dos combos

## ✅ Como salvar

1. Clique com botão direito na foto (no chat ou onde estiver)
2. **"Salvar imagem como..."**
3. Vai pra pasta correta (acima)
4. **Renomeie** com o nome da lista abaixo **EXATO** (tudo minúsculo, sem espaço, terminado em `.webp` ou `.jpg`)
5. Salvar

> 💡 **Dica:** o formato `.webp` é menor e mais rápido. Se sua foto for `.jpg` ou `.png`, salve normal — o código aceita os três.

## 📋 Lista de nomes

### Pizzas 25cm — pasta `images/pizzas/`

| Foto | Nome do arquivo |
|---|---|
| Calabresa (pepperoni vermelho) | `calabresa.webp` |
| Frango c/ Catupiry (com listras brancas) | `frango-catupiry.webp` |
| Portuguesa (presunto + ovo + ervilha) | `portuguesa.webp` |
| Marguerita (tomate + manjericão) | `marguerita.webp` |
| Quatro Queijos (com gorgonzola) | `quatro-queijos.webp` |
| Milho com Bacon | `milho-bacon.webp` |
| Nutellô (chocolate Nutella) | `nutella.webp` |
| Ovomaltine (com flocos) | `ovomaltine.webp` |
| Choc ao Leite (marrom liso) | `choc-leite.webp` |
| Choc Branco (branco/bege) | `choc-branco.webp` |

### Mini — pasta `images/mini/`

| Foto | Nome do arquivo |
|---|---|
| Mini Calabresa (com 4 pepperoni) | `calabresa.webp` |
| Mini Frango c/ Catupiry | `frango.webp` |
| Mini Nutellô | `nutella.webp` |
| Mini Ovomaltine | `ovomaltine.webp` |
| Mini Choc ao Leite | `choc-leite.webp` |
| Mini Choc Branco (cobertura branca lisa) | `choc-branco.webp` |

### Combos — pasta `images/combos/`

| Foto | Nome do arquivo |
|---|---|
| Banner Combo Individual (R$ 26,90) | `individual.webp` |
| Banner Combo Duplo (R$ 49,90) | `dupla.webp` |
| 25cm + Mini + Refri 200ml | `25-mini-refri.webp` |
| 2 Pizzas 25cm + Lata | `2-pizzas-lata.webp` |
| Mini + Coca Mini | `mini-coca.webp` |
| 2 Quadrô Mini | `2-minis.webp` |
| Mini + Kapo | `mini-kapo.webp` |

## 🎯 Depois de salvar

1. Recarregue a página com **Ctrl + F5** (limpa o cache)
2. As fotos aparecem automaticamente em cima do estilo "caixa Quadrô"
3. Se errar o nome, o card mostra o estilo placeholder (não quebra nada)

## 📤 Para publicar online

Depois que salvar todas no seu computador, abra o terminal nessa pasta e rode:

```bash
git add images/
git commit -m "adiciona fotos dos produtos"
git push
```

Em 1-2 minutos o site público também atualiza com as fotos.
