# git

## Базовые команды

- `git init` - инициализировать версионирование репозитория
- `git clone link` - перенести репозиторий по ссылке `link` на локальную машину
- `git add filename` - добавить файл в систему версионирования
- `git commit` - создать слепок текущего состояния репозитория
  - `git commit -m "message"` - добавить сразу сообщение к слепку
- `git push` - перенести текущую версию проекта в удаленный репозиторий
- `git checkout branch/name` - перенестись на другую ветку

## Ветки

- `git branch` - показать текущую ветку
  - `git branch -a` - показать все ветки
- `git branch -m branch/source branch/renamed` - переименование ветки `branch/source` в ветку `branch/renamed`
- `git branch -D branch/to-be-deleted-locally` - удаление локальной ветки с названием `branch/to-be-deleted-locally`
- `git push origin --delete branch/to-be-deleted-remotely` - удаление веткив удаленном репозитории с названием `branch/to-be-deleted-remotely`

## Слияние веток

- `git merge branch/source-for-merge` - слить текущую ветку с веткой `branch/source-for-merge`
- При слиянии веток появляются конфликты. Решать их можно в ручном режиме (проходить по всем файлам и менять на нужное) или же через IDE
