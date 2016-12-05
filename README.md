# Singleton
![Image alt](https://github.com/sergeybushuev/Singleton/raw/master/UML.png)

**Одиночка** - Порождающий шаблон проектирования, гарантирующий, что в однопоточном приложении будет единственный экземпляр некоторого класса, и предоставляющий глобальную точку доступа к этому экземпляру.
## Цель 
 У класса есть только один экземпляр, и он предоставляет к нему глобальную точку доступа. Существенно то, что можно пользоваться именно экземпляром класса, так как при этом во многих случаях становится доступной более широкая функциональность. Например, к описанным компонентам класса можно обращаться через интерфейс, если такая возможность поддерживается языком.

 Глобальный «одинокий» объект — именно объект, а не набор процедур, не привязанных ни к какому объекту — бывает нужен:
- если используется существующая объектно-ориентированная библиотека;
- если есть шансы, что один объект когда-нибудь превратится в несколько;
- если интерфейс объекта (например, игрового мира) слишком сложен и не стоит засорять основное пространство имён большим количеством функций;
- если, в зависимости от каких-нибудь условий и настроек, создаётся один из нескольких объектов. Например, в зависимости от того, ведётся лог или нет, создаётся или настоящий объект, пишущий в файл, или «заглушка», ничего не делающая.

### Плюсы ###
- контролируемый доступ к единственному экземпляру.

### Минусы  
- глобальные объекты могут быть вредны для объектного программирования, в некоторых случаях приводят к созданию немасштабируемого проекта;
- усложняет написание модульных тестов.
