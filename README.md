# our_map
	Наша команда состоит из двух человек: Ботнарь Алины Игоревны и Смертиной Арины Игоревны. 

	Ссылка на карту:https://arinasmertina.github.io/our_map/

	В рамках проекта мы работали с данными по городу Чита - административным центром Забайкальского края, площадью 538 км2 и численностью населения 333 159 чел. (таким образом, плотность населения 619 человек/км2). Город был основан в 1653 году и в 19-20 веке был популярным местом для ссылки декабристов и различных политических преступников. На данный момент, Чита обслуживается 1 аэропортом Кадала, и имеет выгодное транспортное положение за счет расположения на пути Транссибирской магистрали. Сам город разделен на 4 административных района: Черновский, Ингодинский, Центральный, и Железнодорожный. Если посмотреть на расположение объектов культурного наследия, то бОльшая их часть располагается в Центральном районе, несколько объектов в Железнодорожном районе вблизи границ с Центральным.

	В работе нами использовались данные: Таблица формата .СSV с координатами объектов культурного наследия, которые были представлены нам преподавателями (предполагаем, что ими данные были взяты с источников Минкульта); Границы города, скачанные нами из OSM; Слой со зданиями, скачанный из OSM. 

	Первым делом нами была загружена таблица .csv в QGIS, с помощью которой мы получили точечный слой с объектами культурного наследия. Далее с помощью инструмента Join attributes by location были выделены те здания (из выгруженного слоя со всеми зданиями), которые совпадали с точками. Все эти слои были сохранены в формате .geojson. Последующие этапы работы происходили в Visual Studio Code, где была построена сетка 400х400 м2, затем были выбраны ячейки, где непосредственно имеются ОКН и настроена визуализация по количеству этих объектов в ячейках. Далее мы добавили слой с полигонами зданий, для которых были настроены следующие параметры: при наведении курсором появляется название ОКН (используемый для этого инструмент – tooltip); при нажатии появляется год постройки здания (используемый для этого инструмент – popup). Следующим шагом было создание кластерных точек (points cluster), чтобы была возможность смотреть концентрацию объектов ОКН при разном масштабе карты. В конце была добавлена функция управления слоями (Layer Control) для включения или отключения слоев карты, а также функции «Fullscreen» и «Mouse Position» для возможности открытия карты на полный экран и отображения координатов на любую точку карты при наведении курсора.

	В самом начале была сложность, что при выгрузке и наложении слоя с точками из таблицы и слоя со зданиями из OSM многие точки не совпадали и приходилось двигать их вручную. Также была сложность с настройкой визуализации, а именно подбором цветов и масштабов для генерализации.  

	На наш взгляд у нас получилось разобраться и сделать красивую визуализацию,а также удобный и понятный интерфейс для отображения данных по объектам культурного наследия. 

	При работе над проектом все основные задачи были нами выполнены, однако при регистрации на GitHub у одного из членов команды не получилось настроить Pages, так как кнопка «Save» не нажималась, в связи с чем не создавалась ссылка. Понять, почему на одном из компьютеров GitHub не настраивался, понять не удалось.
