flux_reactjs_rus
================

Вольный перевод flux js
http://facebook.github.io/flux/docs/overview.html#content

> Flux applications have three major parts: the dispatcher, the stores, and the views (React components). These should not be confused with Model-View-Controller. Controllers do exist in a Flux application, but they are controller-views — views often found at the top of the hierarchy that retrieve data from the stores and pass this data down to their children. Additionally, actions — dispatcher helper methods — are often used to support a semantic dispatcher API. It can be useful to think of them as a fourth part of the Flux update cycle.

Flux архитектура имеет три составляющие: Dispatcher(диспетчер), Stores(Хранилища) и Views(представления). Представления(views) - это компоненты(components) React'a. Не нужно отображения в архитектуре Flux (flux views) путать со слоем отображения(view layer) модели MVC. Если проводить аналогии с MVC то будет правильно считать, компонеты(components) являются и контроллерами(controller) и отображениями(views) одновременно. Компонеты(component) находящиеся на верху иерархии получают даные из хранилищ(stores) и спускают их вниз по иерархии.

Экшены(actions) - хелпер(helper) методы для диспетчера(dispatcher), нужные для симантической поддержки его API. О них удобно думать как о четвертой составляющей Flux.

> Flux eschews MVC in favor of a unidirectional data flow. When a user interacts with a React view, the view propagates an action through a central dispatcher, to the various stores that hold the application's data and business logic, which updates all of the views that are affected. This works especially well with React's declarative programming style, which allows the store to send updates without specifying how to transition views between states.

Flux - отказ от MVC в пользу архитектуры с однонаправленным потоком данных. Когда пользователь взаимодействует с компонентами React'а (components), они порождают экшены (actions) которые попадают в хранилища (stores) через центральный диспетчер (dispatcher). Хранилища (stores) содержат данные приложения и бизнес логику, а также обновляют все зависимые компоненты (components). Т.е. отображения(views) которые являются компонентами (components) порождают экшены (actions), которые через диспетчер () попадают в хранилища. Хранилища (), обновляют компоненты.
