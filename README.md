# Hyperliquid Builder Viewer

Файлы:

- `hyperliquid_builder_proxy.mjs` — локальный proxy для `stats-data` и `referral`
- `hyperliquid_builder_rebates.html` — HTML-интерфейс с графиком, таблицей и KPI

Запуск:

```bash
cd /Users/mac/Projects/dev30/hyperliquid-builder-viewer
node hyperliquid_builder_proxy.mjs
```

Проверка:

```bash
curl -s http://localhost:8787/health | jq .
```

Если `lz4Available: false`:

```bash
brew install lz4
```

После этого откройте `hyperliquid_builder_rebates.html` в браузере.
