# Cave Floripa — site

Site mobile-first da Cave: loja (natação, bike, corrida, Garmin, Wahoo, CeramicSpeed), fluxo de oferta com cartão pré-autorizado, "venda com a Cave", Bike Fit e locação para provas.

Tudo está em `index.html` (HTML, CSS e JS sem dependências). Para ver, abra o arquivo no navegador.

## Antes de publicar
- Trocar `WA_LOJA` e `WA_FIT` no início do `<script>` pelos números reais (55 + DDD + número).
- Substituir os produtos de exemplo (`RAW`) e os desenhos por fotos reais.
- Definir os preços de locação (hoje "sob consulta").
- Integrar um gateway com pré-autorização (Mercado Pago, Pagar.me ou Stripe) para a oferta e a compra; hoje são demonstração.

## Publicar grátis
GitHub Pages: Settings → Pages → Branch `main` / root. O site fica em `https://<usuario>.github.io/<repo>/`.
