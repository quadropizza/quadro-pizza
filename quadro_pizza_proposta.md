# 🍕 Quadrô Pizza — Proposta de Cardápio Digital

> **A pizza que nasceu pra ser diferente** · Retangular · Artesanal · Insana  
> Univali Itajaí · Bloco C2 · Ao lado do Teatro

---

## 📋 Visão Geral

Cardápio digital em HTML único — sem app, sem instalação, sem mensalidade.  
O cliente abre pelo celular, monta o pedido e confirma direto pelo WhatsApp.  
O proprietário acessa um painel protegido por senha para ver o resumo da semana.

---

## 🎯 Funcionalidades do Cliente

### Tela de Entrada
- Pop-up de boas-vindas solicitando o nome do cliente
- Nome salvo no dispositivo — na próxima visita aparece **"Que bom te ver, [NOME]!"**
- Identidade visual da marca: vermelho, amarelo e preto

### Navegação
| Aba | Conteúdo |
|-----|----------|
| 🔥 Combos | Combos em destaque com imagem, descrição e seletor de sabores |
| 🍕 Pizza 25cm | Todos os sabores salgados e doces com foto |
| 🍕 Mini | Sabores disponíveis no formato mini |
| 🥤 Bebidas | Latas, águas, Kapo e Del Valle agrupados |

### Cardápio

**Quadrô 25cm — R$ 19,99**
- Salgadas: Calabresa, Frango c/ Catupiry, Portuguesa, Marguerita, Quatro Queijos, Milho c/ Bacon
- Doces: Nutellô, Ovomaltine, Choc. ao Leite, Choc. Branco

**Quadrô Mini — R$ 12,90**
- Salgadas: Calabresa, Frango
- Doces: Nutellô, Ovomaltine, Choc. ao Leite, Choc. Branco

**Combos**
| Combo | Itens | Preço |
|-------|-------|-------|
| ⚽ Individual Copa 2026 | Pizza 25cm + Refri Lata + 1 Figurinha | R$ 26,90 |
| ⚽ Dupla Copa 2026 | 2 Pizzas 25cm + Refri Lata + 2 Figurinhas | R$ 49,90 |
| 🔥 25cm + Mini + Refri | Pizza 25cm + Mini + Refri 200ml | R$ 26,90 |
| 👫 2 Pizzas 25cm + Lata | 2 Pizzas + Refrigerante Lata | R$ 36,90 |
| 💥 Mini + Coca Mini | Mini + Coca-Cola 200ml | R$ 14,90 |
| ✌️ 2 Quadrô Mini | 2 Minis à escolha | R$ 22,90 |
| 🥤 Mini + Kapo | Mini + Kapo 200ml | R$ 14,90 |

**Figurinhas FIFA 2026 (somente PIX)**
| Quantidade | Preço/pacote |
|-----------|-------------|
| Até 10 pct | R$ 6,90 |
| Acima de 10 pct | R$ 6,80 |
| Acima de 50 pct | R$ 6,50 |

### Fluxo de Pedido
1. Cliente navega e adiciona itens ao carrinho
2. Clica em **Finalizar Pedido**
3. Escolhe entrega:
   - **Retirar no Balcão** — Bloco C2, agora ou horário agendado (08h–22h)
   - **Entrega na Sala** — exclusivo alunos CAU 1° ao 5° ano, apenas nos intervalos **08h50** ou **15h00**
4. Escolhe pagamento: PIX · Débito · Crédito · Dinheiro
   - PIX: chave CNPJ `60.723.998/0001-84` com botão copiar
   - Figurinhas aceitam **somente PIX**
5. Clica **Confirmar via WhatsApp** — mensagem completa enviada automaticamente

### Mensagem WhatsApp (modelo)
```
*NOVO PEDIDO - QUADRÔ PIZZA*
---------------------------------------
*Olá, Lucas!* Recebemos seu pedido:

*Pedido #123456*  |  06/05/2026 às 14:30

*ITENS:*
----------------------
1. *Individual Copa 2026* -- *R$ 26,90*
   -> Sabor da Pizza 25cm: Frango c/ Catupiry
   -> Refrigerante Lata: Coca-Cola
----------------------
*TOTAL: R$ 26,90*

*ENTREGA:* Retirar no Balcão (Bloco C2)
*QUANDO:* Agora (~5 minutos)
*PAGAMENTO:* PIX

*CHAVE PIX (CNPJ):*
60.723.998/0001-84
_Envie o comprovante nesta conversa!_

Obrigado, Lucas! Pizza pronta em ~5 min! 🔥
```

### Pós-venda
- 20 segundos após o pedido aparece pop-up de avaliação (1–5 estrelas + comentário)
- Avaliação enviada via WhatsApp para o número da loja
- Histórico de todos os pedidos do dispositivo salvo localmente

---

## 🔐 Painel do Proprietário

Acesso via botão discreto no rodapé do cardápio: **"Área do Proprietário"**

### Login
- Usuário: `quadro`
- Senha: definida pelo proprietário (armazenada com hash no localStorage)
- Sessão expira em 8 horas

### Dashboard — Resumo da Semana

#### Visão Geral (cards de topo)
| Card | O que mostra |
|------|-------------|
| 💰 Faturamento | Total em R$ dos pedidos da semana |
| 📦 Pedidos | Quantidade total de pedidos |
| 🍕 Ticket Médio | Faturamento ÷ pedidos |
| ⭐ Avaliação Média | Média das estrelas recebidas |

#### Gráficos
- **Pedidos por dia** — barra com os últimos 7 dias
- **Faturamento por dia** — linha com os últimos 7 dias
- **Forma de pagamento** — pizza: PIX / Débito / Crédito / Dinheiro

#### Ranking de Itens
- Top 5 itens mais pedidos na semana com quantidade e % do total

#### Avaliações Recentes
- Lista das últimas 10 avaliações com nome, nota e comentário

#### Filtros
- Semana atual / Semana passada / Últimos 30 dias

> **Obs:** todos os dados vêm do localStorage do dispositivo onde os pedidos foram  
> confirmados. Para uso em múltiplos dispositivos, recomenda-se versão com backend.

---

## 📱 Informações da Loja

| Campo | Valor |
|-------|-------|
| WhatsApp | (47) 99766-1485 |
| Localização | Ao lado do Teatro da Univali — Bloco C2 |
| Tempo de preparo | ~5 minutos |
| Instagram | @quadropizzaa |
| Chave PIX | 60.723.998/0001-84 (CNPJ) |

---

## 🛠 Especificações Técnicas

| Item | Detalhe |
|------|---------|
| Formato | Arquivo `.html` único, sem dependências externas |
| Hospedagem | Qualquer serviço estático (GitHub Pages, Netlify, etc.) |
| Compatibilidade | Chrome, Safari, Firefox · Desktop e mobile |
| Armazenamento | localStorage — dados ficam no dispositivo do usuário |
| Tamanho do arquivo | ~600 KB (imagens comprimidas embutidas) |
| Integrações | WhatsApp Web API (wa.me) |
| Analytics | Painel proprietário interno (sem Google Analytics) |

---

## 🚀 Próximos Passos Sugeridos

- [ ] Integração com sistema de pagamento PIX automático
- [ ] Painel em nuvem para acesso de múltiplos dispositivos
- [ ] Notificações push quando chegar novo pedido
- [ ] QR Code para o cardápio impresso nas embalagens
- [ ] Módulo de fidelidade (ex: a cada 10 pizzas, 1 grátis)

---

*Proposta elaborada em maio de 2026 · Quadrô Pizza · Univali Itajaí*
