# forumalem

Конкурс на лучший форум / блог для сайта [alem.school](https://alem.school). Команда победителей получит призы от teamalem, уважение от студентов и развернет свой форум для внутреннего и внешнего использования. 

## Условия оценивания

- Чистый код
- Правильная структура проекта
- Безопасность: авторизация, токены, валидации
- UI/UX: удобство и адаптивность
- Архитектура базы данных

___


## Техническое задание

Минимальные требования к проекту:
* Авторизация / Регистрация через OAuth2 Gitea
* Главная страница с постами, ссылками:
  * со всех досок
  * с досок, на которые подписан пользователь (а-ля reddit)
* Доски (раздел):
  * подписка
  * поиск по постам
  * сортировка
      * дата
      * популярность
  * создания постов, комментариев
* Пост / Комментарий
  * возможность встраивать картинки
  * встраивать ссылки
  * форматирование кода [пример](https://i.imgur.com/arsDIrr.png)
  * сохранение, изменение, удаление
* Реакции
  * отметки нравится / не нравится к постам / комментариям
  * умный алгоритм "популярности" постов / комментариев по реакциям
* Страница пользователя
  * информация из gitea
  * карма
  * последние посты, комментарии

## Важно

Максимальное количество участников в команде - 5 человек.

Проект должен иметь MIT лицензию.

Проект должен запускаться в Docker контейнере.

В проекте должна быть папка `scripts` со следующими файлами.
```sh
__forum
 |....
 |___scripts
      |- start.sh  # запуск проекта
      |- reload.sh # перезапуск проекта (для обновления)
      |- stop.sh   # остановка проекта
```

start.sh и reload.sh должны принимать аргумент и запускать/перезапускать на указанном порту.

Пример:
```sh
export PORT=8080
sh start.sh $PORT
sh reload.sh $PORT
```

___

## Условия участия

1. Делаете pull request в файл [participants.md](https://github.com/alem-01/forumalem/edit/master/participants.md)
2. Добавляете новую линию следующим форматом:
```sh
https://git.01.alem.school/atlekbai/forum - atlekbai, Adilyam, Zulbukharov, sakenism
```

Нужно отправить ссылку на репозиторий и логины сокомандников через запятую.

3. Ждете апрува от teamalem

