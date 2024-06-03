# doc-qa
🇬🇧 [English](README-en.md)

Телеграм бот для поиска по документам с помощью `LangChain`. Сделан в рамках хакатона для данных, находящихся под NDA.

## Прогресс

- [x] Класс `Retriever` для загрузки файлов и работы с `LangChain`, имеющий метод `answer` для вывода цитаты, отдела документа и ссылки на документ по заданному вопросу.
- [x] Прототип бота.
- [x] Тесты с выводом метрик.
- [x] `Docker` контейнер.
- [x] Добавление новых документов в векторное хранилище.
- [ ] Авторизация в бот.
- [ ] Указание отдела для поиска при задавании вопроса.

## Данные ПЭК
Для использования проекта с данными ПЭК, скачайте все предоставленные файлы `zip` архивом, переименуйте архив в `data.zip`, поместите его в папку `data` репозитория, далее следуйте инструкции по установке и запуску.

## Установка и запуск
```
git clone https://github.com/molokhovdmitry/doc-qa
cd doc-qa
```
Переименуйте файл `.env.example` в `.env`, укажите в нем токен для телеграм бота и путь к архиву с данными.
```
pip install -r requirements.txt
python -m spacy download ru_core_news_lg
python -m src.bot
```
