
# Варіант №11

Завдання:

    1.Потрібно вивчити теоретичний матеріал та написати власноруч приклад коду для патерну decorator. 
    Деяку теоретичну інформацію можна почерпнути тут https://refactoring.guru/uk/design-patterns/decorator
    2.Закомітити приклад НАПИСАНИЙ власноруч та зробити pull request.
    3.Згідно власного варіанту потрібно переписати існуючий проект та додати за потреби нові класи. 
    Варіанти завдань отримати у викладача.
    3.В README файлі навести UML діаграму класів для коду згідно власного варіанту з короткими поясненнями.
    4.Закомітити код та зробити pull request.

Завдання згідно з варіантом:

    Декоратор для даних JSON в XML Створити декоратор, який конвертує дані в форматі JSON в XML для спрощення інтеграції з іншими системами.
    
## UML діаграма класів
![diagram.png](obj%2Fimg%2Fdiagram.png)
### Класи та інтерфейси:

- **IDataConverter**: Інтерфейс, який визначає метод ConvertData, який буде реалізований класами конвертерів даних.
- **JsonConverter**: Конкретна реалізація інтерфейсу IDataConverter для конвертації даних в JSON.
- **DataConverterDecorator**: Абстрактний клас декоратора, який реалізує інтерфейс IDataConverter та містить посилання на об'єкт типу IDataConverter. Цей клас може бути розширений конкретними декораторами.
- **JsonToXmlDecorator**: Конкретний декоратор, який конвертує дані з JSON в XML. Він наслідується від DataConverterDecorator та додає специфічну функціональність конвертації даних.

### Застосування:

Застосування декоратора для конвертації даних з JSON в XML може бути корисним у випадках, коли потрібно інтегрувати систему, яка працює з JSON, з іншими системами, що очікують дані у форматі XML.
