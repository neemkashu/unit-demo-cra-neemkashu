# WARNING

```
Прошу проверить мою работу в среду
🙏
```

<details>
  <summary>Нажмите, чтобы посмотреть детали реализации</summary>

В репозитории настроен `CI`.

Изменения в ветке `master` происходят только через пулл реквесты.

В ПР происходят проверки:

- сообщений коммитов на пуш
- сообщений всех коммитов в ПР
- прогон е2е и юнит тестов

Пока все проверки не пройдены, ПР не может быть замержен.

Пример валидного ПР ✅ [ссылка](https://github.com/neemkashu/unit-demo-cra-neemkashu/pulls)

Пример невалидного ПР ❌ [ссылка](https://github.com/neemkashu/unit-demo-cra-neemkashu/pull/9): падает тест и проверка коммита

### Релиз

Релиз иницируется при пуше тега вида `v*`, где `*` -- какое-то число

- Автоматически создаётся issue с заголовком `RELEASE version v*`, в котором находится информация о
  - инициаторе релиза
  - списке коммитов с предыдущего релиза
  - дате начала релиза (или перезапуске, если тег повторно запушен)
- Создаётся ветка вида `release-v*` от коммита с релизным тегом
- Для деплоя необходим ручной запуск `workflow` по решению ответственного человека (_один из варинтов реализации релиза по лекции_).
  Для запуска выберите `Run workflow` на странице с экшенами [ссылка](https://github.com/neemkashu/unit-demo-cra-neemkashu/actions/workflows/deploy.yml)

### Команды

```sh
# установить зависимости
npm ci

# запустить приложение
npm start

# запустить тесты е2е
npm run e2e

# запуск модульных тестов
npm test
```

Чтобы пропустить локальную валидацию сообщения коммита

```sh
# bash
HUSKY=0 git commit -m 'non valid message'
```

</details>
