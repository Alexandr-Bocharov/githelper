# Как создать файл локально и разместить версию на гитхаб, если вы уже работали на гитхаб

## Создаем файл

1. Открываем терминал  
2. Заходим в домашнюю директорию с помощью команды cd ~  
3. Создаем __папку__ с помощью команды mkdir 'название папки'  
4. Создаем __файл__ touch 'название файла'  
5. Редактируем __файл__ при необходимости  

## Закидываем версию на гитхабыч

1. Возвращаемся в терминал  
2. Прописываем git add 'название файла' (_подготовили файл к сохранению/коммиту_)  
3. Прописываем там же в терминале git commit -m (Комментарий к сохранению, в кавычках) - _Сохранили подготовленый файл_  
4. Прописываем в терминале get push (Отправляем версию файла на гитхаб)  
5. Готово

## Дополнительные сведения  
Подробный курс по работе с гит и гитхаб есть на [ЯндексПрактикум](https://practicum.yandex.ru/git-basics/?from=catalog 'Да, да, ЖМЯКАЙ!')

---

# Хэш/хэширование

Хеш - уникальный номер коммита, который представлен в 16-ричной системе счисления. Состоит из 40 символов

## Как узнать хэш коммита
Хэши коммитов можно узнать, если введете в папке, которая инициализирована гитом, - _git log_  
Если хотите узнать хэш последнего коммита:  
1. cd .git && cat refs/heads/main _или же cat refs/heads/master

Если хотите узнать краткую информацию по коммитам:  
- git log --oneline  

# HEAD

В папке __.git__ имеется файл HEAD, в котором хранится ссылка на хэш последнего коммита.  
Благодаря этой ссылке и команде 'cat' мы можем отобразить сам хэш.

