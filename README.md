## Цепочка наследования стандартных классов в JavaScript

****

:information_source: Данное приложение представляет собой инструмент для разработчика, который предоставляет удобный интерфейс для просмотра полной цепочки наследования стандартных классов в JavaScript. </p>
Позволяет вывести полную цепочку прототипов для любого класса, который содержится в глобальном объекте Window (например, *HTMLInputElement, History*).
Кроме этого это приложение обрабатывает ошибки. В том числе, при вводе названия класса, отсутствующего в Window, сообщение об ошибке появляется не в консоли, а под полем ввода.

Этим ресурсом удобно пользоваться в процессе изучения JS.

2. **Как работает интерфейс программы Prototype chain JS Window:**
   + Пользователь в поле `input` пишет название класса или модуля (с учетом регистра) и нажимает кнопку `Показать цепочку прототипов`
   + Осуществляется валидации заполненных данных, если `Данный класс отсутствует в Window` или `Данное свойство не является функцией-конструктором`, надо написать верный класс
   + При успехе, на экране появляются данные в виде:
   + 
     ```
      Object
      1. Название свойства - "toString". Тип свойства - function`
      ```

:information_source: В этом приложении мы ищем класс, который содержится **в глобальном объекте Window**.    
Window - это глобальный объект JavaScript. Для обращения к объекту Window существует свойство window, которое является ссылкой на объект.
   
   Window является глобальным объектом JavaScript и содержит в себе другие объекты. Например, **объект document** принадлежит объекту Window.
   
   В JavaScript есть и другие объекты принадлежащие объекту Window. Например, **объект Screen**, который содержит информацию об экране пользователя (например, о его разрешении).
   Объект History отвечает за «историю», то есть за информацию о том, как пользователь перемещался по сайту.
   
   Таким образом, объект Window является «родителем» для других объектов. Но в основном о нём не упоминается.

:information_source: Изучая язык JS важно разобраться с тонкосятми работы прототипов. 
+ В JavaScript объекты имеют специальное **скрытое свойство** `[[Prototype]]`, которое является либо другим объектом, либо null.
+ Можно использовать obj.__proto__ [`__proto__`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/proto) для доступа к нему.
+ Объект, на который ссылается [[Prototype]], называется «прототипом».

:sos: Подробнее изучить тему прототипов в JavaScript -> [Прототипное наследование](https://learn.javascript.ru/prototype-inheritance) 

Технологический стек: JavaScript, Bootstrap, HTML.