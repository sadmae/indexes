# Доверие и регулирование: модель Кыргызстана

Интерактивная модель (по Aghion, Algan, Cahuc, Shleifer, 2010), откалиброванная по данным Кыргызстана.
Статическая страница `public/index.html`, публикуется как Cloudflare Worker со статическими ассетами.

## Деплой

```bash
cd trust-model
npx wrangler@4 deploy
```

Для неинтерактивного окружения нужен `CLOUDFLARE_API_TOKEN` с правом «Workers Scripts: Edit».
