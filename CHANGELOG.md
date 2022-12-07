# Change Log

## [2022.10.p3](https://github.com/lord-server/lord/releases/tag/2022.10.p3)
 - Fixes #873. Replace registered_player -> minetest.player_exists (#875)
 - Fixes 799. Check if item is registered, if it's not, return nil (#876)

## [2022.10.p2](https://github.com/lord-server/lord/releases/tag/2022.10.p2)
 - Fixes #865. Slightly renew nickname filter algorithm (#870)

## [2022.10.p1](https://github.com/lord-server/lord/releases/tag/2022.10.p1)
 - Исправлены бесконечные стаки дерева (#813, #814)

## [2022.10](https://github.com/lord-server/lord/releases/tag/2022.10)
 - Добавлены призрачные блоки для шерсти (#576, #737)
 - Добавлены плиты из стволов деревьев (#698, #739, #757, #765, #766)
 - Добавлены расширенные подсказки в описаниях в инвентаре, книжках и др формах (#589)
   Сейчас отображается:
   - Урон для топоров, мечей, кинжалов и др. оружия
   - Свечение для факелов, свеч и др. излучающих нод
   - Макс. урон для стрел и метательных топоров
 - Добавлены овцы и возможность стричь их (#769)
 - При обновлении Lottblocks добавлены (#771, #342):
   - Сундук гномов
   - Мифриловая лампа
   - Гонг
 - Добавлен штандарт Шира. (#358, #781)
 - Добавлены расовые двери (#789)
 - Добавлен урон от воды Мордора (#771, #342)
 - Добавлено "Ведро с водой Мордора" (#771, #342)
 - Исправления/доработки:
   - Исправление автоматического срубания дерева. (#756, #758)
   - Исправление дна расовых сундуков (#791)
   - Теперь после выпивания зелья остаётся бутылка (fixes #100) (#761)
   - Добавлены боковые текстуры люков из тех же пород дерева (#792)
 - Рефакторинг/системное:
   - Removed ping mod (#746)
   - Moved overwriting strings.lower, upper to lordlib mod (#745)
   - Moved palantiri storage from text file to mod meta (fixes #751) (#753)
   - Moved lottpotion from _lott/ to lord/ :building_construction: (#718) resolves #715
   - Add core_callbacks (#699)
   - stale-bot: decrease days until stale
   - Unify debug tools (#747)
   - Updated ambience with submodule (fixes #161)
   - #267 Update MTG/default: insignificant changes (#763)
   - Lottblocks update (#771) closes #342
   - Beautify README (#775)
   - Lottblocks i18n: Migration to built-in translation system (#776) Resolves #772
   - Add basic definitions for built-in functions and tables (#778)
   - EditorConfig: same rules as \`*.lua\` for \`.luacheckrc\`
   - MTG/doors update (#708)
   - CI: Deploy WFs: add `--recurse-submodules` to fix deploy
   - Implemented races.can_open_stuff (#787)
   - Рефакторинг `defaults:` (#790)
   - lottmapgen_update: refactoring chest spawners
   - lottmapgen_update: removed mythical fog
   - lottplants_update: moved overwrites to correct place
   - lottmapgen_update: changed localization to built-in
   - Switch some MTG mods to submodules. Relates to #601. All switched mods from 5.4.1 commit (42baede):
     - beds - downgrade to 5.4.1 (removed: check player attached, locale/beds.eo.tr)
     - bucket
     - carts
     - doors
     - dye
     - farming
     - fire
     - downgrade to 5.4.1 (locale/fire.eo.tr deleted)
     - flowers
     - player_api
     - screwdriver
     - sethome
     - sfinv
     - stairs
     - vessels
     - wool
   - correct GH-actions for work with submodules
   - CI: increase `actions/checkout` `fetch-depth` (fix build)

## [2022.08.p3](https://github.com/lord-server/lord/releases/tag/2022.08.p3)
 - Added green marble stairs and slabs (fixes #762) (#764)

## [2022.08.p2](https://github.com/lord-server/lord/releases/tag/2022.08.p2)
 - Исправлено падение сервера при разрушении трупа
 - Исправлен перевод блока льда

## [2022.08.p1](https://github.com/lord-server/lord/releases/tag/2022.08.p1)
 - Исправление исчезнувших ступенек сена (#742) fixes #741.

## [2022.08](https://github.com/lord-server/lord/releases/tag/2022.08)
 - добавлены серебряные, стальные и оловянные лампы (#548);
 - заменена текстура берёзы (#692);
 - орочья еда больше не вредит оркам (fixes #656) (#681);
 - новые реечные заборы (#602 и #706);
 - lord bees (#623):
   - добавлен блок воска
   - добавлен блок медовых сот
   - добавлены фоны диалоговых окон ульев и центрифуги
   - обновлены текстуры центрифуги
   - имитация вылета пчёл из ульев (вылетают только при наличии матки)
 - добавлены блоки мрамора (#574):
   - Marble with gold
   - Marble with gems
 - Исправление ошибок:
   - исправлен баг с запятыми в имени палантира (fixes #189) (#668);
   - исправлено неправильное покачивание (waving) листвы (fixes #660) (#673);
   - отмычка больше не расходует ресурс в creative #170 (#666 😈)
   - удален несуществующий в мире `default:bush_leaves` (fixes #650) (#684);
   - исправлен баг с негаснущими под водой факелами (fixes #551) (#693);
 - Администраторские:
   - команда `/list`:
     - добавлен поиск по minetest'овской локализации (fixes #419) (#669);
     - реализован поиск по нажатию Enter;
     - переработка и чистка кода;
     - призрачные ноды перенесены в конец списка;
   - убрана возможность выкинуть админский жезл (fixes #367) (#647)
   - призрачные ноды убраны из меню креатива
 - Рефакторинг/системные:
   - переработка "расовых" сундуков (#666 😈);
   - обновление lottplants (fixes #350) (#328);
   - небольшая переработка lord_money (#652)
   - переработка lord_boats (fixes #535) (#615);
   - реализована вспомогательная функция lord.give_or_drop (fixes #597) (#675);
   - реализована вспомогательная функция `lord.each_value_equals` (fixes #688) (#689);
   - `mega_sl` теперь использует mod security (fixes #594) (#695);
   - чистка устаревших depends.txt и других предупреждений (#614 и #712);
 - Экспериментальные:
   - добавлен инструмент lord_replacer (#713 и #720)

## [2022.07.p3](https://github.com/lord-server/lord/releases/tag/2022.07.p3)
 - Fix iron chest craft with default:chest (fixes #690) (#691)

## [2022.07.p2](https://github.com/lord-server/lord/releases/tag/2022.07.p2)
 - Fix leaf decay with using default.register_leafdecay (fixes #662) (#677)
 - Fix bug with endless rails (fixes #627) (#672)
 - Fix papyrus growth (fixes #670) (#671)

## [2022.07.p1](https://github.com/lord-server/lord/releases/tag/2022.07.p1)
 - Enable tree decay on both types of trunks (#657)

## [2022.07](https://github.com/lord-server/lord/releases/tag/2022.07)
 - Добавлен новый блок: зелёный мрамор. Доступен только на официальных прилавках (#571)
 - Новая иконка игры L.O.R.D. #518 (#604)
 - Обновление текстур:
   - Брусчатки (#567)
   - Кристалов и драг. камней (#577)
   - Руд в инвентаре (#570)
   - Бумаги, бумаги с текстом, лицензии магазина (#618)
 - Обновления модов:
   - `MTG/flowers` #278 (#488)
   - `MTG/carts` #273 (#531) + #642 (#645)
   - `MTG/sethome` #573 (#580)
   - `MTG/default`: upd nodes.lua, functions.lua & trees.lua #267 (#563) + #631 (#632) + #636 (#644)
   - `MTG/farming` #276 (#453) + #630 (#655, #643)
   - Добавлен `MTG/sfinv` #634 (#635)
 - Исправление ошибок:
   - Восстановлен декоративный кактус #488 (#566)
   - Fix Mount-gen fill: Place dirt where air or plantlike #607 (#608)
   - Fix warnings in logs #362 (#612)
   - Доработка работы формы рабочего стола (#622)
   - `lottmobs`: add previously skipped tnt texture. fix (#372) (#616)
   - Fix crash when player leaves after drinking wine (fixes #291) (#649)
   - Fix sound & textures for ice. Closes #626 (#633)
   - Use `default.chest.get_chest_formspec()` in LOTT chests (fixes #653) (#654)
 - А также:
   - Removing temporary changes in `MTG/stairs`. Fixes #510 (#603)
   - Add nodes_dump as a submodule #588 (Closes  #586)
   - New PR template (#638, #639, #641)
   - Move luacheck from Travis CI to GitHub Actions (fixes #526) (#648)


## [2022.02.p4](https://github.com/lord-server/lord/releases/tag/2022.02.p4)
 - Check nodes for their existence in areas (#617)

## [2022.02.p3](https://github.com/lord-server/lord/releases/tag/2022.02.p3)
 - New coal and charcoal textures (#591)
 - Classic textures (#592)
 - marble texture (#593)
 - Fixes mountain tool (#537, Closes #425)
 - Update mount tool (#606, relates to #547)

## [2022.02.p2](https://github.com/lord-server/lord/releases/tag/2022.02.p2)
 - Fix LuaCheck build. (Fixes #578)
 - Fix pearl transparency #559 (#579)
 - Fix crosshair.png symmetry. Add object_crosshair.png (#581)
 - Fix wooden axe #461 (#583)
 - Add Diamond Block stairs & slabs #437 (#584)
 - Fix new player hunger #383 (#585)

## [2022.02.p1](https://github.com/lord-server/lord/releases/tag/2022.02.p1)
 - Исправления багов:
   - Check that mob is not nil when punch #555 (#556)
   - Fix arrow collision calculation #542 (#545)
 - Релизный процесс:
   - Always switch back to master on deploy
   - Reconfigure ci: `dev` branch to polygon; version tags to prod & tags can have patch segment
   - reconfigure ci: add merge master to dev on deploy to prod; add release description
 - Перенос модов с сервера в репозиторий (#305)
   - Copy mod `skybox` from prod server. Relates to #305.
   - Copy mod `arena` from prod server. Relates to #305
   - Copy mod `alarm` from prod server. Relates to #305
   - Copy mod `painting` from prod server. Relates to #305
   - Copy mod `ping` from prod server. Relates #305
   - Copy mod `server_message` from prom server. Relates to #305
   - Copy mod `ambience` from prod server. Relates to #305
   - Copy mod `lists` from prod server. Relates to #305
   - Copy mod `mail_list` from prod server. Relates to #305
   - Copy mod `mobs_fish` from prod server. Relates to #305
   - Copy mod `mypos` from prod server. Relates to #305
   - Copy mod `sethome` from prod server. Relates to #305

## [2022.02](https://github.com/lord-server/lord/releases/tag/2022.02)
 - Обновлён мод `MTG/beds`. Исправлен #312 сброс скорости после сна (#429)
 - Обновлён мод `MTG/vessels` #281 (#506)
 - Обновлён мод `MTG/dye` #275 (#507)
 - Обновлён мод `MTG/wool` #281 (#509)
 - Обновлён мод `MTG/screwdriver` #280 (#516)
 - Обновлён мод `MTG/player_api` #279 (#528)
 - Обновление и перенос мода `MTG/boats` в `lord/lord_boats` #270 (#534)
 - Частично обновлён мод `MTG/default` #267:
   - удалены дублирующие ступеньки и плиты из `pine_wood`
   - добавлен блок из песчаника `sandstone_block` (добавлены, но пока не доступны `desert_sandstone`, `desert_sandstone_brick`, `desert_sandstone_block`)
   - добавлена mese-лампа `meselamp`
   - добавлены обсидиановые кирпич `obsidianbrick` и блок `obsidian_block`
   - добавлен каменный блок `stone_block` (добавлен, но пока не доступн `desert_stone_block`)
   - add `default:large_cactus_seedling` & grow funcs, move `default:dirt` recipe
   - добавлено изготовление камня `default:stone` из замшелого булыжника `default:mossycobble` и пустынного камня `default:desert_stone` из пустынного булыжника `default:desert_cobble`
   - перебалансировка топлива:
     - из разных стволов деревьев (стволы разных пород горят разное время)
     - из разных досок
     - из разных саженцев
     - из разных заборов
     - и некоторых других вещей
   - добавлены, не пока недоступны сухая трава `dry_grass_#`, папоротник `fern_#`, песчаный тростник `marram_grass_#`
 - Добавлены переводы для inner & outer stairs #508 (#511)
 - Добавлен инструмент для построения графа зависимостей модов dependency graph (#363)
 - Исправление кроватей в данжах #500 (#502)
 - Исправление расположения текстур #432 (#494)
 - Исправлена бесплатная починка в магазинах `lord_money` #512 (#536)
 - Исправлен краш при смерти моба #538 (#539)
 - Исправлен краш при выстреле амбразуры #540 (#541)
 - Исправлено падение при поиске в книгах крафта #497 (#496, #544)
 - Перенесён мод `bones` из MTG в lord. Fixes #271 (#486)
 - Перенесено всё, что относится к `charcoal` в наш внутренний мод `lord_default`. (требуется для #267) (#491)
 - Переход на minetest `5.4.1`:
   - Исправления по устаревшему API #499, #498, #286, #285, #505, #409 (#501, #503, #412, #549)
 - Hotfix: Fix screwdriver #554

## [2021.11](https://github.com/lord-server/lord/releases/tag/2021.11)
 - Добавлены новые блоки для дорог с бордюром (#381)
 - Добавлены новые лампы в золотой и бронзовой окантовке (#465)
 - Добавлено отображение цены и товара у менялы (#450)
 - Добавлена `is_creative_enabled` для дальнейшего перехода на 5.4. Во избежание #438
 - Ранее встроенный в `MTG/fire` мод `campfire` вынесен в отдельный мод. (Closes #455)
 - Обновлён `MTG/fire`. (Closes #277)
 - Обновлён `MTG/bucket`. (Closes #272)
 - Удалён неиспользуемый мусор: `lord.mod_loaded`, `lord.load`, `lordlib/signals.lua` (`lord.emit`, `lord.on`) (#475)
 - Добавлена информация о contributor'ах и инфа о code-style
 - Исправление отображения текста на табличках (таблички требуется переустановить)
 - Исправление падения при прожигании неизвестной ноды (#436)
 - Исправление бага с менялой (Fixes #413)
 - Quick-fix при обновлении `MTG/fire`: удалён звук для синего пламени (#480)

## [2021.09](https://github.com/lord-server/lord/releases/tag/2021.09)
 - Обновление мода `lottclothes` из LoTT (последнее)
 - Перенос `lottclothes` в папку `lord`
 - Обновлена модель: теперь отображается одежда
 - Отображение скина в инвентаре (#338)
 - Исправление отображения скина при первоначальном выборе расы новым игроком (отображается тень) (#398)
 - Добавлен админский магазин (#314)
 - Игрокам Оркам стало легче жить и добывать в шахтах: гномы теперь не спаунятся при оркских факелах, но спаунятся оркри, тролли и пауки (#360)
 - Обновлены текстуры слитков
 - Конфигуратор для горного посоха (#396)
 - Ускорение работы горного посоха (#424)
 - Добавлены новые блоки для Полосатого гномьего камня: с одной полосой и с двумя на одной плоскости
 - Подготовка к обновлению сервера: Переход на встроенную систему переводов MT в папке `lord` (#367) (#328)
 - Исправление падения сервера при входе в "Справку" (#393)
 - Исправление поиска на русском для встроенной системы переводов MT

## [2021.08](https://github.com/lord-server/lord/releases/tag/2021.08)
 - Доработки для дальнейшего перехлда на версию 5.3
 - Явное разделение стандартных, наших и сторонних модов и добавлено описание
 - Обновление `MTG/stairs`
 - Добавлено описание `development.md` для разработчиков с минимальными инструкциями
 - Исправлен баг в установке areas
 - Обновление `lottpotion` из LOTT. Relates to #288
 - Исправление стрел с зельями #288 #289
 - Исправлена ошибка #264 'Unknown node: `lottblocks:dwarf_bottom`'
 - Набросок тулзы для создания гор (пока не используем) (#293) beta version
 - Появился админский доступ к магазинам
 - Исправление полёта стрел (#292 #299 #300)
 - Добавлено отображение HP на Арене (ID=2316) (#301)
 - Мод `spawn` добавлен в основной репозиторий на GH
 - Добавлена команда `/death` и унифицирован механизм спаунов (#309 #327 #369)
 - Добавлен инфо-моб и моб-меняла (#307 #306 #334 #333)
 - Настраиваимый спаун для разных рас #311
 - Обновление мода `MTG/default`: текстуры, звуки, модельки, переводы, вынесены наши изменнеия; у сундуков поднимается крышка и многое другое
 - Исправлена высота посадки на лошадь
 - Обновление `lottarmor` из lott и вынесение в папку `lord`
 - Улучшение Барлога: увеличина скорость fireball'а, не поражают друг друга
 - Добавлена команда `/dice` - выдаёт случайное число
 - Хоббиты получают урон на земле мордора. Closes #310
 - На Тень теперь не наподают мобы

## [2021.01](https://github.com/lord-server/lord/releases/tag/2021.01)
 - Обновлено API игрока
 - Исправлены модели мобов
 - Улучшения кактуса и тростника (можно рубить нижний, верхние срубаются автоматически)
 - Обновлён мод stairs: добавлены угловые блоки, теперь [можно так](https://github.com/lord-server/lord/issues/253).
 - Добавлены скрипты авто выкладки на тестовый и боевой сервера
 - Исправлены ошибки с отсутствующими текстурами (добавлены из minetest_game)

## [2020.04](https://github.com/lord-server/lord/releases/tag/2020.04)
- Исправления: Перевод на новый API игрока из Minetest 5.x DefaultGame
- Исправлена опечатка: "Заменитель мордерского камня" -> "Заменитель мордорского камня"

## [2019.12](https://github.com/lord-server/lord/releases/tag/2019.12)
 - Обновлён мод `carts`: ЖД звуки, повороты на развилках
 - Добавлены участники проекта в `readme.md`
 - Исправлена ошибка #250: в книгах крафта при повторном поиске не сбрасывалась страница
 - Исправлена ошибка: падение при первом открытии книги доспехов
 - Добавлена секция `Contributing / Помощь проекту` в `readme.md`
 - Для NPC включен таймер жизни
 - Добавлена Ель
 - Добавлен Навес
 - Добавлены Стойки
 - Обновлены тележки

## [2019.11](https://github.com/lord-server/lord/releases/tag/2019.11)
 - Добавлены ступеньки и плиты для стекла
 - Поиск в книгах "Основы крафта" и "Все рецепты"
 - Добавлена поддержка "фракций" (Если вы орк, вас атакуют люди, эльфы и пр.; если вы человек или эльф, то вас атакую орки, варги и пр.)
 - Изменена текстура мордорского камня
 - Исправлены белые мобы
 - В `readme.md` добавлены секции: о сервере L.O.R.D.; список `contributors` с ролями; секция `Contributing` о том как помочь проекту
 - Добавлены шаблоны для описания ошибки (bug'а) и для описания идеи (feature request)
 - Исправлена загрузка настроек creative_mode (подгружаем только один раз)

## [2019.10](https://github.com/lord-server/lord/releases/tag/2019.10)
 - Правки модели игрока под версию 5.*
 - Правки моделек мобов под версию 5.*
 - Правки HUD под версию 5.*
 - Индикация здоровья мобов
 - Уничтожение мобов со здоровьем меньше 0
 - Обновление `chatcommands` из нового LOTT

## [2019.01](https://github.com/lord-server/lord/releases/tag/2019.01)
 - Появились котята и мышата
 - Появились орки-лучники
 - Изменились текстуры топоров и крекера
 - Добавлены звуки металла
 - Исправлена цена у тогрговцев
 - Исправление работы печей и дробилки
 - Исправления в сталактитах
 - Исправлено отображение превью кольца воды в инвентаре
 - Исправление установки ствола дерева на пьедестал
 - Хот-фикс с боевого: проверка сети палантира
 - Переписан движок стрельбы/метания
 - Арбалеты, луки и пр. перенесено на новый движок
 - Рефакторинг использования кеша в расах
 - Рефакторинг дробилки
 - Использование функций для звуков металла и гравия
 - Удаление лишних алиасов, лишнего кода, лишних крафт схем, текстур
 - Исправления опечаток в названиях блоков и предметов (бутыльки)
 - Добавлена интеграция с Travis для прогона LuaCheck
 - Вычищен код по всем замечаниям от LuaCheck
 - Убрано использование устаревшей `intllib.Getter()`
 - Добавлена иконка к игре
