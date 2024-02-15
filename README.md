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

## Rebase

- `git rebase branch/name` - перенести текущую ветку на ветку `branch/name`
- `git rebase --abort` - отменить процесс переноса
- `git rebase --continue` - используется после решения конфликтной ситуации, продолжает процесс переноса
- `git rebase --skip` - используется для подхвата изменений из ветки `branch/name`
