<details> <summary><strong>📄 Clique para expandir o conteúdo do README</strong></summary>
# 🥙 Sistema Administrativo - Esfiharia

Projeto completo de painel administrativo + loja para gerenciamento e venda de esfihas, inspirado em VTEX/Shopify.

---

## 🧱 Estrutura do Banco de Dados

- **Usuários (`User`)**: nome, e-mail, senha, tipo (admin, atendente, entregador)
- **Produtos (`Product`)**
- **Categorias (Departamento > Categoria > Subcategoria)**
- **Pedidos (`Order`)** com status (Recebido, Em preparo, Pronto, Entregue)
- **Clientes (`Customer`)**
- **Financeiro (relatórios futuros)**
- **Cupons (`Coupon`)**
- **Entregas (`DeliveryZone`)**
- **Editor de conteúdo (`SiteContent`)**

---

## 🚀 Tecnologias Sugeridas

- **Frontend Admin + Loja:** Next.js + Tailwind CSS
- **Backend/API:** Node.js + Express
- **Banco de Dados:** PostgreSQL + Prisma ORM
- **Autenticação:** JWT
- **Integrações futuras:** WhatsApp, Mercado Pago, Pix

---

## 🔐 Níveis de Acesso

- **Admin**: acesso total
- **Atendente**: produtos, pedidos, clientes
- **Entregador**: pedidos e entregas

---

## 🛠️ Rotas REST principais

- `POST /auth/login`
- `GET /products` / `POST /products`
- `GET /orders` / `PATCH /orders/:id`
- `GET /customers`
- `POST /coupons`
- `GET /site-content`
- etc...

---

## 📲 Integração com WhatsApp

- Enviar mensagens automáticas ao mudar o status do pedido
- Exemplo de fluxo:
  - Pedido confirmado
  - Pedido saiu para entrega

---

## 📅 Roadmap

### 🟢 Fase 1: Estrutura inicial
- [x] Modelagem do banco
- [x] Planejamento do painel admin

### 🔵 Fase 2: Admin dashboard
- [ ] Login com JWT
- [ ] CRUD de produtos e categorias
- [ ] Pedidos com alteração de status

### 🟡 Fase 3: Loja (frontend)
- [ ] Catálogo de produtos
- [ ] Carrinho e checkout
- [ ] Integração com backend

---

## 📌 Observações

- O projeto está sendo desenvolvido do zero, com foco em escalabilidade e flexibilidade.
- Estrutura inspirada em plataformas como VTEX, Shopify e Tray.
</details>
