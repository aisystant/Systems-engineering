---
title: 'Альфа инженерных обоснований: акцент на фиче/инкременте'
---

Обоснование --- это описание системы с точки зрения её успешности. Так
что альфа инженерного обоснования и все её подальфы --- это подальфы
описания, а рабочие продукты этих описаний --- это assurance case,
«папка обосновывающего дела», как папка судебного дела или дела/досье в
какой-нибудь канцелярии, то есть документ (сегодня это обычно набор
записей в базе данных, а не «листок бумаги» или даже «листок бумаги в
электронной форме, например .pdf файл»).

Во всех стандартах чётко говорится, что обоснование успешности системы
(QA, обоснование качества) должно вестись в ходе всей разработки
системы. Выделение «испытаний» как обособленной стадии жизненного цикла
(работ проведения испытаний, когда все остальные работы не ведутся) всё
менее и менее оправдано, ибо испытания частей (юнит-тесты, которые пишут
сами разработчики) ведутся задолго до интеграционных испытаний, а после
начала эксплуатации (это происходит с каждой фичей, с каждым «железным»
изделием в серии, возможно каждое изделие в серии будет другое) эти же
испытания ведутся так же регулярно (скажем, самодиагностика во время
включения у оборудования, в котором есть хоть какой-то
микропроцессор --- это уже обычное дело, и помним про манифест
прочности: система всё время себя оценивает, что с ней происходит, чтобы
быть прочной). А ещё в инженерных обоснованиях всё начинается сильно
раньше испытаний, и rationale тоже документируют, включая rationale на
старт самого проекта создания системы. То есть считать обоснование
«стадией» нельзя, это сразу получается длиной в целый жизненный цикл,
это практика, которую ведут в ходе всей разработки, укрепляя и укрепляя
уверенность в том, что система получается успешной, **на неё можно
положиться** (dependable, ещё одно часто используемое слово для
выражения претензии/claim на успешность/success --- и это архитектурная
характеристика).

При непрерывном вводе в эксплуатацию обосновывается по факту и каждая
новая фича/инкремент, но и обосновывается, что вся система будет
работать с этой новой фичей. Так что в начале проекта формулируется
претензия на успешность MVP, и дальше накапливаются материалы, её
обосновывающие (подчинённые претензии в их иерархии/subclaims, аргументы
и доказательства). В целом состояния, которые должна пройти альфа
обоснований (включая её подальфы, например, связанные с обоснованием для
отдельных частей системы) могут быть такими (приводим вариант и системы,
и фичи как отдельного инкремента, реализуемого в ходе непрерывной
разработки. Если это фича, то весь цикл от замысла до введения в
эксплуатацию может занимать и один день):

-   Система/фича будет нужна --- претензия на нужность системы
    обоснована (инвестиционное или технико-экономическое обоснование
    концепции использования, rationale)
-   Система/фича технически и экономически возможна --- претензия на
    достижимость результатов проекта обоснована (концепция системы
    обоснована, rationale, архитектура обоснована, результаты могут быть
    оттестированы/юнит-тесты написаны)
-   Система/фича спроектирована --- представлены rationale по принятым
    проектным и архитектурным решениям, код написан/информационная
    модель для завода подготовлена/решения для персонала предприятия
    (если целевая система --- предприятие) приготовлено. Можно
    изготавливать (работа DevOps).
-   Система/фича отмоделирована и испытана --- получены свидетельства
    для обоснования успешности системы (и фичи, и всей системы).
-   Система/фича успешна --- получено полноценное инженерное обоснование
    успешности системы (для собранных свидетельств построены аргументы,
    обосновывающие претензию на успешность системы, аргументы
    приняты --- это делается при обоснованиях успешности по compliance
    со стандартами, и изредка при обоснованиях продолжения проекта для
    топ-менеджеров, занимающихся стратегированием).

Как видите, тут большой соблазн поставить альфу обоснования как подальфу
коммерческой возможности (тем более что первый пункт прямо относится к
коммерческой возможности ведения проекта по созданию системы или
микропроекта одной команды по созданию/модификации новой фичи для
системы). Это вполне возможно, ибо альфы представляют собой не дерево, а
граф, подальфа вполне может быть подальфой двух альф (это особо
оговаривается и в стандарте OMG Essence). Но учитываем, что:

-   все состояния альф ссылаются друг на друга (это особо обговаривается
    в стандарте OMG Essence), это лишний повод обратить внимание
    организации проекта на важность удерживать отслеживание проектной
    ситуации по всем альфам в их взаимосвязи, нет требования иметь
    «ортогональные независимые» альфы
-   онтологическая строгость определения альф и подальф не слишком
    большая. Каждая организация проекта адаптирует альфы к своей
    проектной ситуации до уровня мета-модели (предметной области из
    культуры, «как в учебниках» и предметной области «как у нас в
    проекте», то есть согласно регламентам и стандартам предприятия и
    предпочтениям сотрудников организации проекта). Так что нужно
    смотреть на то, как обычно устроены обоснования в вашей предметной
    области, но наш курс и упомянутая в нём литература даст много идей о
    том, что может быть там пропущено или наоборот, что может быть
    лишним в силу лоббирования «безопасников».

Один из студентов-бакалавров предыдущей версии курса на вопрос, что ему
пригодилось больше всего из материала, сказал: «я понял из курса, что
есть проверка и приёмка. И я начал проверять всё, что выходит из моих
рук перед тем, как отдавать работу. И моя жизнь драматически изменилась
к лучшему». **Не ленитесь делать инженерные обоснования** **с самого
начала до самого конца проекта, и ваша жизнь тоже драматически изменится
к лучшему!** **Но будьте готовы, что на это уйдёт половина вашего
времени, а то и больше!**
