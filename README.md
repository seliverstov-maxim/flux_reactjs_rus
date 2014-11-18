flux_reactjs_rus
================

Вольный перевод flux js
http://facebook.github.io/flux/docs/overview.html#content

> Flux applications have three major parts: the dispatcher, the stores, and the views (React components). 
These should not be confused with Model-View-Controller. Controllers do exist in a Flux application, 
but they are controller-views — views often found at the top of the hierarchy that retrieve data from 
the stores and pass this data down to their children. Additionally, actions — dispatcher helper 
methods — are often used to support a semantic dispatcher API. It can be useful to think of them as a 
fourth part of the Flux update cycle.

Flux архитектура имеет три составляющие: Dispatcher(диспетчер), Stores(Хранилища) и Views(представления).
Представления(views) - это компоненты(components) React'a. Не нужно отображения в архитектуре Flux (flux views) 
путать со слоем отображения(view layer) модели MVC. Если проводить аналогии с MVC то будет правильно считать, компонеты(components) являются и контроллерами(controller) и отображениями(views) одновременно. 
Компонеты(component) находящиеся на верху иерархии получают даные из хранилищ(stores) и спускают их вниз по иерархии.

Экшены(actions) - хелпер(helper) методы для диспетчера(dispatcher), нужные для симантической поддержки его API.
О них удобно думать как о четвертой составляющей Flux.
