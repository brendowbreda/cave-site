# Cave Floripa — site

Site mobile-first da Cave (preto e branco): loja de natação, bike, corrida, Garmin, Wahoo e CeramicSpeed, fluxo de oferta com cartão pré-autorizado, "venda com a Cave", Bike Fit e locação para provas.

## Estrutura
- `index.html` — o site.
- `admin/` — área do administrador (cadastrar, editar, marcar como vendido, configurações).
- `data/products.json` — produtos (editado pelo admin).
- `data/config.json` — WhatsApp, oferta mínima, preços do Bike Fit e da locação, categorias.
- `img/products/` — fotos enviadas pelo admin.
- `assets/` — logo, favicon e desenhos usados quando um produto não tem foto.

## Área do administrador
Abra `https://brendowbreda.github.io/cave-site/admin/` e entre com uma chave de acesso do GitHub:

1. GitHub → Settings → Developer settings → Personal access tokens → **Fine-grained tokens** → Generate new token.
2. Repository access: **Only select repositories** → `cave-site`.
3. Permissions → Repository permissions → **Contents: Read and write**.
4. Gere, copie e cole no login do admin.

Cada alteração vira um commit no repositório e o GitHub Pages atualiza o site em cerca de 1 minuto.

Produto **vendido**: a foto fica borrada em preto e branco, o preço aparece como `R$ *****,**` e ficam só título e subtítulo.

## Pendências
- Números reais de WhatsApp (hoje são de teste; troca em Admin → Configurações).
- Preços da locação (Admin → Configurações).
- Pagamento online com pré-autorização (Mercado Pago, Pagar.me ou Stripe). Hoje Comprar e Fazer oferta finalizam pelo WhatsApp.

## Ver localmente
O site carrega os dados com `fetch`, então precisa de um servidor: `python3 -m http.server` na pasta e abra `http://localhost:8000`.
