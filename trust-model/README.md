# Доверие и регулирование: модель Кыргызстана

Интерактивная модель (по Aghion, Algan, Cahuc, Shleifer, 2010), откалиброванная по данным Кыргызстана.
Статическая страница `public/index.html`, публикуется как Cloudflare Worker со статическими ассетами.

## Деплой

Основной адрес: https://trustmodel-kg.pages.dev (Cloudflare Pages, проект `trustmodel-kg`).

```bash
cd trust-model/public
npx wrangler@4 pages deploy . --project-name trustmodel-kg --branch main
```

Запускать из папки без `wrangler.jsonc`: иначе wrangler 4 считает проект воркером.
Нужен `CLOUDFLARE_API_TOKEN` с правами на Workers и Pages.

Вариант на Workers (адрес содержит поддомен аккаунта): `cd trust-model && npx wrangler@4 deploy`.
