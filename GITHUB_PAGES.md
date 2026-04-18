# GitHub Pages deploy

Под публикацию нужен только статический approve UI.

Файлы для репозитория/ветки Pages:
- `index.html`
- `.nojekyll`

Минимальные шаги:
1. Создать публичный GitHub repo.
2. Залить `index.html` и `.nojekyll` в корень репозитория.
3. В GitHub открыть `Settings -> Pages`.
4. В `Build and deployment` выбрать `Deploy from a branch`.
5. Выбрать ветку `main` и папку `/ (root)`.

После публикации страница будет доступна по `https://<user>.github.io/<repo>/`.

Важно:
- кошелек должен открывать страницу по `https://`, не через `file://`
- для approve-страницы backend не нужен
- локальный `hyperliquid_builder_proxy.mjs` для GitHub Pages не используется
