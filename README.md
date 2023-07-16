# WARNING

```
Прошу проверить мою работу в среду
🙏
```

<details>
  <summary>Нажмите, чтобы посмотреть детали реализации</summary>
  
  В репозитории настроен CI.

Изменения в ветке `master` происходят только через пулл реквесты.

В ПР происходят проверки:

- сообщений коммитов на пуш
- сообщений всех коммитов в ПР
- прогон е2е и юнит тестов

Пока все проверки не пройдены, ПР не может быть замержен

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
