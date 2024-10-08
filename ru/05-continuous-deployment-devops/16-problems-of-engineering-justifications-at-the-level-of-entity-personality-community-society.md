---
title: Проблемы инженерных обоснований на уровне существа, личности, сообщества, общества
---

Многочисленные проблемы появляются в тех случаях, когда мы выходим в
инженерию других видов систем, и вот несколько примеров:

-   Проектирование финансов предприятия, сводящееся к бюджетированию.
    Обычно оно связано с разработкой бюджета, а затем исполнением
    бюджета, что занимает годичный цикл. Движение **beyond**
    **budgeting** и аналогичные
    ему^[<https://corporate-rebels.com/beyond-budgeting-model/>]
    представляет собой по факту попытку сделать **непрерывное**
    **бюджетирование** по модели DevOps, где сначала вместо годичного
    цикла (за год может случиться и скачок цен на продукцию, и уход
    надёжных поставщиков материалов, и скачки в валютных курсах, и
    забастовки, и наоборот --- новые открытия, которые дают новые
    коммерческие возможности, но строгий годичный бюджет не даст
    возможность выжить в этих условиях) идут «итерации» бюджетирования
    «скользящим окном» сначала квартальным, потом месячным, но затем всё
    переходит к непрерывному бюджетированию, где разные части бюджета
    непрерывно дорабатываются, публикуются как план расходов, а потом
    происходит контроль исполнения бюджета, и в случае явных ошибок идёт
    быстрое изменение бюджета.
-   При покупке предприятий, при заключении крупных сделок обычно
    проводят процедуры проверки **due**
    **diligence**^[<https://en.wikipedia.org/wiki/Due_diligence>],
    чтобы убедиться в отсутствии каких-то неприятных сюрпризов, которые
    могут произойти после завершения сделки. Это тоже инженерное
    обоснование, «входной контроль», но речь идёт о личностях и
    организациях, и возникает сразу много интересных особенностей. Как
    минимум, полностью меняется терминология, полностью меняются
    процедуры, а ещё это разовое действие --- хотя и тут возможны
    варианты, по ходу проекта ведь сразу начинается организационное
    развитие уже совместного (после
    M&A^[<https://en.wikipedia.org/wiki/Mergers_and_acquisitions>],
    merges and acquisitions) предприятия.
-   Если речь идёт о **показаниях** и высказываемых в них
    претензиях/claims отдельных людей, то как могут быть устроены
    обоснования? Врёт или не врёт человек, может быть проверено на
    детекторе лжи, который сам по себе может врать или не врать,
    надёжность такого «доказательства» очень низка. Можно использовать
    «сыворотку правды», хотя это по факту конспирология (набор легенд) и
    вряд ли работает с надёжностью выше
    случайности^[[https://ru.wikipedia.org/wiki/Сыворотка\_правды](https://ru.wikipedia.org/wiki/Сыворотка_правды)],
    причём можно и попросту пытать «по старинке», хотя пытки --- метод
    «испытаний» тоже не самый надёжный и полученное под пытками или даже
    угрозами пыток свидетельство/evidence в основу аргумента сегодня не
    положишь, поэтому и обосновать мало что получится. Тут сразу
    поднимается множество вопросов об этике методов получения
    свидетельств/улик/показаний/замеров, включая «судебный
    поединок»^[[https://ru.wikipedia.org/wiki/Судебный\_поединок](https://ru.wikipedia.org/wiki/Судебный_поединок)]
    как ранее считавшийся вполне SoTA методом и сводящийся к дуэли. И
    вот мы получили вроде как свидетельства/улики/evidence такими
    сомнительными методами. Как оценивать результаты, как строить
    аргумент, если заранее известно, что свидетельство ненадёжно?
    Никакой же статистики для отдельных людей по отдельным вопросам
    набрать нельзя, а должны же быть вопросы про false positive и false
    negative заключения, ибо от ложных обоснований как positive, так и
    negative могут быть весьма драматические последствия (скажем,
    пожизненное заключение невиновных на основе ложных обоснований,
    сделанных судом). Всегда нужно помнить, что на любой плохой метод
    инженерного обоснования можно вспомнить метод ещё хуже, и по факту
    используются все эти методы, иногда и в одном проекте.
-   **Клинические
    испытания**^[<https://en.wikipedia.org/wiki/Randomized_controlled_trial>],
    которые массово проводятся прямо сейчас в порядке реализации идеи
    «доказательной медицины», представляются нерациональными, их нельзя
    считать получением надёжных
    обоснований^[<https://ftp.cs.ucla.edu/pub/stat_ser/r513.pdf>].
    Дело в том, что получаемая статистика относится к группе людей, а
    назначение лекарства после испытания получает один человек, а не
    группа. И при текущем положении дел с методами аргументирования
    классической статистикой проведением клинических испытаний даже
    двойным слепым методом ничего сказать про персональное назначение
    препарата потом нельзя, но можно сказать методами причинного
    вывода/causal inference. По большому счёту, вся сегодняшняя
    «доказательная медицина» построена на песке, она ничего не
    доказывает (вернее, доказывает, но совсем не то, что нужно для
    инженерной части: для предсказуемого изменения мира), малопонятно,
    что с этим делать. Причинный вывод сегодня мало кем понимается, хотя
    он и решает множество имеющихся проблем. Впрочем, и текущий вариант
    причинного вывода нельзя считать последним словом: он опирается на
    расчёт байесовской, а не квантовоподобной вероятности, то есть
    заведомо даёт искажённый по сравнению с реальностью
    результат^[<https://ailev.livejournal.com/1619025.html>].
    Тут есть ещё один интересный момент: если у вас больной заведомо
    умрёт, но есть минимальный шанс, что выживет, если вы дадите ему
    потенциально опасное лекарство, которое ещё не прошло клинических
    испытаний ни по какой методике (скажем, просто не успели): вы будете
    испытывать это лекарство на таком больном, и это будет лечение или
    испытание? А если вы оставите каких-то больных «контрольной группы»
    без этого лекарства, они ж заведомо умрут! Этично ли это? Вопросы
    множатся и множатся.
-   **Обоснование успешности обучения** как инженерное обоснование
    какого-то мастерства. Подробней этот вопрос поднимается в курсе
    «Образование для образованных», но вывод там печальный: экзамены
    обычно не показывают успешности обучения, кроме самых простых
    случаев элементарных навыков. Диплом вуза не показывает успешности в
    работе, результаты ЕГЭ не показывают успешности в жизни. Более того,
    большие проблемы с «экзаменами» как методом получения свидетельств
    для обоснования успешности создания машинного интеллекта, то есть
    «испытания» тут непонятно как сделать.
-   **Обоснование идей по социальной инженерии** поднимает те же вопросы
    «экспериментов на людях». При этом даже в случае получения
    отрицательных результатов (например, все случаи сознательного
    устройства общества на основе социалистических идей были провальны,
    но попытки продолжаются и продолжаются, несмотря на «отрицательный
    результат испытаний», под лозунгом «они там всё неправильно делали,
    а вот у нас непременно получится!»). Одно из решений тут --- ход на
    классический либерализм как обобщение хода, выработанного в ходе
    Реформации и кровопролитных религиозных войн католиков и гугенотов:
    они там все разрешили друг другу маршировать прямо в ад, ибо честно
    считали, что именно это и происходит, но прекратили насаждать путь в
    рай военным путём. Поэтому кто хочет маршировать прямо в
    социалистический голод и диктатуру (как считают одни) или
    социалистический рай (как считают другие) --- пусть марширует, если
    не втягивает в это других людей, это неплохое начало. Но если это
    реальная социальная инженерия, а не допотопная эволюция, то неплохо
    бы для начала получить какие-то обоснования. И тут оказывается, что
    как и для клинических испытаний, как для экзаменов «готовности к
    жизни», как для «интеллекта» каких-то надёжных методов обоснования
    успешности социального инженерного проекта нет. Это не значит, что
    нельзя предлагать каких-то «умных мутаций» и как-то пытаться
    выделить их результаты среди всего многообразия жизненных явлений
    (легко ведь сделать и неверные выводы: «100% из попробовавших в
    своей жизни огурцы людей рано или поздно умерли. Значит, огурцы
    вредны, статистика не может врать!»).
