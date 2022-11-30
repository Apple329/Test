# test
<!doctype html>
<html>
<head>
<meta charset="utf-8">
<title>Untitled Document</title>
<style type="text/css">
<!--
body {
	line-height: 1.2;
	font-size: 132%;
	font-family: Segoe, "Segoe UI", "DejaVu Sans", "Trebuchet MS", Verdana, sans-serif;
	background-color: #3511E9;
	margin: 0;
	padding: 0;
	color: #FFFFFF;
	background-image: url(
%D0%B8%D0%B7%D0%BE%D0%B1%D1%80%D0%B0%D0%B6%D0%B5%D0%BD%D0%B8%D1%8F/446716_myagkie_legkie_svetlye_1680x1050_(www.GdeFon.ru).jpg);
	border-color: #001DFF;
	font-style: normal;
	font-weight: bold;
	text-indent: 0px;
	text-shadow: 0px 0 #000000;
	background-image: url(%D0%B8%D0%B7%D0%BE%D0%B1%D1%80%D0%B0%D0%B6%D0%B5%D0%BD%D0%B8%D1%8F/luxfon.com-4527.jpg);
	right: auto;
}
/* ~~ Element/tag selectors ~~ */
ul, ol, dl { /* Due to variations between browsers, it's best practices to zero padding and margin on lists. For consistency, you can either specify the amounts you want here, or on the list items (LI, DT, DD) they contain. Remember that what you do here will cascade to the .nav list unless you write a more specific selector. */
	padding: 0;
	margin: 0;
}
h1, h2, h3, h4, h5, h6, p {
	margin-top: 0;	 /* removing the top margin gets around an issue where margins can escape from their containing block. The remaining bottom margin will hold it away from any elements that follow. */
	padding-right: 15px;
	padding-left: 15px; /* adding the padding to the sides of the elements within the blocks, instead of the block elements themselves, gets rid of any box model math. A nested block with side padding can also be used as an alternate method. */
	font-weight: bold;
	text-align: justify;
}
a img { /* this selector removes the default blue border displayed in some browsers around an image when it is surrounded by a link */
	border: none;
}
/* ~~ Styling for your site's links must remain in this order - including the group of selectors that create the hover effect. ~~ */
a:link {
	color: #FFFFFF;
	text-decoration: underline; /* unless you style your links to look extremely unique, it's best to provide underlines for quick visual identification */
}
a:visited {
	color: #443EFF;
	text-decoration: underline;
}
a:hover, a:active, a:focus { /* this group of selectors will give a keyboard navigator the same hover experience as the person using a mouse. */
	text-decoration: none;
	color: #443EFF;
	text-align: center;
}
/* ~~ This fixed width container surrounds all other blocks ~~ */
.container {
	width: 960px;
	background-color: #FFFFFF;
	margin: 0 auto; /* the auto value on the sides, coupled with the width, centers the layout */
}
/* ~~ The header is not given a width. It will extend the full width of your layout. ~~ */
header {
	background-color: #ADB96E;
}
/* ~~ These are the columns for the layout. ~~ 

1) Padding is only placed on the top and/or bottom of the block elements. The elements within these blocks have padding on their sides. This saves you from any "box model math". Keep in mind, if you add any side padding or border to the block itself, it will be added to the width you define to create the *total* width. You may also choose to remove the padding on the element in the block element and place a second block element within it with no width and the padding necessary for your design.

2) No margin has been given to the columns since they are all floated. If you must add margin, avoid placing it on the side you're floating toward (for example: a right margin on a block set to float right). Many times, padding can be used instead. For blocks where this rule must be broken, you should add a "display:inline" declaration to the block element's rule to tame a bug where some versions of Internet Explorer double the margin.

3) Since classes can be used multiple times in a document (and an element can also have multiple classes applied), the columns have been assigned class names instead of IDs. For example, two sidebar blocks could be stacked if necessary. These can very easily be changed to IDs if that's your preference, as long as you'll only be using them once per document.

4) If you prefer your nav on the left instead of the right, simply float these columns the opposite direction (all left instead of all right) and they'll render in reverse order. There's no need to move the blocks around in the HTML source.

*/
.sidebar1 {
	float: left;
	width: 180px;
	background-color: #EADCAE;
	padding-bottom: 10px;
}
.content {
	padding: 10px 0;
	width: 600px;
	float: left;
	text-align: center;
	color: #FFFFFF;
	font-family: marvel;
	font-style: normal;
	font-weight: 400;
}
aside {
	float: left;
	width: 180px;
	background-color: #EADCAE;
	padding: 10px 0;
}

/* ~~ This grouped selector gives the lists in the .content area space ~~ */
.content ul, .content ol {
	padding: 0 15px 15px 40px; /* this padding mirrors the right padding in the headings and paragraph rule above. Padding was placed on the bottom for space between other elements on the lists and on the left to create the indention. These may be adjusted as you wish. */
}

/* ~~ The navigation list styles (can be removed if you choose to use a premade flyout menu like Spry) ~~ */
nav ul{
	list-style: none; /* this removes the list marker */
	border-top: 1px solid #666; /* this creates the top border for the links - all others are placed using a bottom border on the LI */
	margin-bottom: 15px; /* this creates the space between the navigation on the content below */
}
nav li {
	border-bottom: 1px solid #666; /* this creates the button separation */
}
nav a, nav a:visited { /* grouping these selectors makes sure that your links retain their button look even after being visited */
	padding: 5px 5px 5px 15px;
	display: block; /* this gives the link block properties causing it to fill the whole LI containing it. This causes the entire area to react to a mouse click. */
	width: 160px;  /*this width makes the entire button clickable for IE6. If you don't need to support IE6, it can be removed. Calculate the proper width by subtracting the padding on this link from the width of your sidebar container. */
	text-decoration: none;
	background-color: #C6D580;
}
nav a:hover, nav a:active, nav a:focus { /* this changes the background and text color for both mouse and keyboard navigators */
	background-color: #ADB96E;
	color: #FFF;
}

/* ~~ The footer ~~ */
footer {
	padding: 10px 0;
	background-color: #CCC49F;
	position: relative;/* this gives IE6 hasLayout to properly clear */
	clear: both; /* this clear property forces the .container to understand where the columns end and contain them */
}
/* ~~ Miscellaneous float/clear classes ~~ */
.fltrt {  /* this class can be used to float an element right in your page. The floated element must precede the element it should be next to on the page. */
	float: right;
	margin-left: 8px;
}
.fltlft { /* this class can be used to float an element left in your page. The floated element must precede the element it should be next to on the page. */
	float: left;
	margin-right: 8px;
}
.clearfloat { /* this class can be placed on a <br /> or empty block element as the final element following the last floated block (within the .container) if the footer is removed or taken out of the .container */
	clear:both;
	height:0;
	font-size: 1px;
	line-height: 0px;
}

/*HTML 5 support - Sets new HTML 5 tags to display:block so browsers know how to render the tags properly. */
header, section, footer, aside, article, figure {
	display: block;
}
a:hover {
	color: #443EFF;
}
a:active {
	color: #443EFF;
}
-->
</style><!--[if lt IE 9]>
<script src="http://html5shiv.googlecode.com/svn/trunk/html5.js"></script>
<![endif]-->
<meta name="" content="">
<meta name="keywords" content="Конон М.В.">
<!--The following script tag downloads a font from the Adobe Edge Web Fonts server for use within the web page. We recommend that you do not modify it.--><script>var __adobewebfontsappname__="dreamweaver"</script><script src="http://use.edgefonts.net/artifika:n4:default;modern-antiqua:n4:default;marvel:n4:default;ubuntu-mono:n4:default;medula-one:n4:default.js" type="text/javascript"></script>
</head>

<body text="#3200FF">
<table width="912" border="1" align="center">
  <tbody>
    <tr>
      <td width="556" height="111"><img src="изображения/Шапка.jpg" alt="" width="903" height="168" align="middle"/></td>
    </tr>
    <tr>
      <td height="52"><table width="904" border="1">
        <tbody>
          <tr>
            <td width="88" bgcolor="#FFFFFF"><div align="center"><a href="MAIN PAGE.html">Главная</a></div></td>
            <td width="116" bgcolor="#FFFFFF"><div align="center"><a href="1.html">Введение</a></div></td>
            <td width="116" bgcolor="#FFFFFF"><div align="center"><a href="2.html">Глава 1</a></div></td>
            <td width="115" bgcolor="#FFFFFF"><div align="center"><a href="3.html">Глава 2</a></div></td>
            <td width="141" bgcolor="#FFFFFF"><div align="center"><a href="4.html">Заключение</a></div></td>
            <td width="288" bgcolor="#FFFFFF"><div align="center"><a href="5.html">Список источников</a></div></td>
          </tr>
        </tbody>
      </table></td>
    </tr>
    <tr>
      <td height="1900"><table width="904" border="1">
	  <p>2 ПОИСК ИНФОРМАЦИИ. АНАЛИТИЧЕСКИЙ ОБЗОР НАЙДЕННЫХ ДОКУМЕНТОВ</p>
      <p>При поиске информации были использованы такие поисковые машины, как: </p>
      <p>- <a href="https://www.google.by">https://www.google.by</a>/; </p>
      <p>- <a href="http://www.yandex.by/">http://www.yandex.by/</a></p>
      <p>и другие. </p>
      <p>Также был использован режим «расширенный поиск», который имеет каждая из названных поисковых систем. В качестве ключевых слов сначала вводилась полностью тема, как на русском, так и на иностранных языках, а именно на английском. Затем более узко, например, «Коробка передач», «Главная передача», «Диагностирование».  Проведем аналитический обзор найденных документов по теме «Диагностирование коробок передач и главных передач». </p>
      <p>1.	<a href="https://cyberleninka.ru/article/n/vosstanovlenie-detaley-vazhnyy-rezerv-ekonomii-resursov/viewer ">Ссылка </a></p>
      <p>В.П. Лялякин, доктор технических наук, ГНУ ГОСНИТИ Россельхозакадемии </p>
      <p>ВОССТАНОВЛЕНИЕ ДЕТАЛЕЙ - ВАЖНЫЙ РЕЗЕРВ ЭКОНОМИИ РЕСУРСОВ  </p>
      <p>Приведены технико-экономические показатели восстановления деталей, дан анализ состояния восстановления деталей в России и за рубежом, показана перспектива восстановления. </p>
      <p>Ключевые слова: деталь, восстановление, изнашивание, упрочняющие технологии. </p>
      <p>2.	<a href="https://cyberleninka.ru/article/n/vliyanie-modulya-silikata-na-tehnologicheskie-svoystva-peo-pokrytiy/viewer">Ссылка </a></p>
      <p>А.В. Косенко, В.А. Казански, инженеры, Ариэльский Университетский Центр Самарии, Израиль</p>
      <p>Ю.А. Кузнецов, доктор технических наук, ФГОУ ВПО Орел ГАУ </p>
      <p>ВЛИЯНИЕ МОДУЛЯ СИЛИКАТА НА ТЕХНОЛОГИЧЕСКИЕ СВОЙСТВА ПЭО ПОКРЫТИЙ  </p>
      <p>Плазменно-электролитическое оксидирование (ПЭО) позволяет получить на вентильных металлах покрытия, значительно изменяющие свойства поверхности. В этой работе изучался процесс оксидирования при использовании натриевых силикатов (жидких стекол) различных модулей "n" (где n-стехиометрический индекс в обобщенной формуле силиката натрия Na2O-nSiO2). </p>
      <p>Ключевые слова:	плазменно-электролитическое оксидирование (ПЭО), силикат натрия, алюминиевый сплав, микротвердость, плотность тока. </p>
      <p>3.	<a href="https://cyberleninka.ru/article/n/organizatsiya-remonta-i-vosstanovleniya-rabotosposobnosti-detaley-mashin/viewer">Ссылка </a></p>
      <p>Е.А. Кудряшов, д-р техн. н., профессор, зав. каф. «Технология машиностроения», ЧитГУ, А.В. Стецурин, аспирант каф. «Технология машиностроения», ЧитГУ </p>
      <p>ОРГАНИЗАЦИЯ РЕМОНТА И ВОССТАНОВЛЕНИЯ РАБОТОСПОСОБНОСТИ ДЕТАЛЕЙ МАШИН </p>
      <p>В работе приведен анализ дефектов деталей машин автотранспортного общемашиностроительного назначения, возникающих в процессе эксплуатации. </p>
	  <p>Обобщен опыт исследований в области восста¬новления работоспособности изношенных деталей машин  </p>
      <p>Ключевые слова: ремонт, восстановление, работоспособность </p>
      <p>4.	<a href="https://cyberleninka.ru/article/n/entropiya-v-ranzhirovanii-metodov-vosstanovleniya-detaley/viewer ">Ссылка </a></p>
      <p>В. Г. Петряков, В. С. Наталенко, М. М. Маннанов, И. Р. Ахметьянов </p>
	  <p>ЭНТРОПИЯ В РАНЖИРОВАНИИ МЕТОДОВ ВОССТАНОВЛЕНИЯ ДЕТАЛЕЙ </p>
      <p>Объектом исследования является сравнительная оценка методов восстановления деталей с применением энтропийного алгоритма и на этой основе осуществлять оптимизацию квалиметрии восстановления деталей. </p>
	  <p>Целью работы является получение количественных результатов сравнительной оценке методов восстановления. </p>
	  <p>Для сравнительной количественной оценке качества используется ранжирование методов восстановления деталей по отдельным единичным показателям качества, формирующих качество изделия в целом. Предложен алгоритм энтропийной функции оценки качества, в котором наилучшее упорядочение системы, её равновесное состояние достигается при максимуме энтропии с учётом заданных ограничений на затраты. </p>
	  <p>Алгоритм энтропийной функции позволяет моделировать, сравнивать альтернативные варианты и на этой основе осуществлять разработку, ранжирование и оптимизацию многосложных структур продукции с неограниченным числом показателей. </p>
	  <p>Применение данного алгоритма автоматизировано и реализовано в системе Mathcad. </p>
	  <p>По результатам его применения дана количественная сравнительная оценка методов восстановления и сформирован вариационный ряд значений энтропийной функции откуда следует, что по технологическим показателям лучшей суммарной результативностью обладают практически два метода: электроконтактная приварка стальной ленты и наплавка под слоем флюса. </p>
	  <p>Таким образом, применение энтропийной функции в ранжировании методов восстановления позволяет объективно принимать управленческое решение в применении конкретного метода и образовывать ожидаемое качество восстановленных деталей. </p>
      <p>Ключевые слова: восстановление, работоспособность </p>
      <p>5.	<a href="https://cyberleninka.ru/article/n/razrabotka-ratsionalnyh-tehnologicheskih-shem-uprochneniya-i-vosstanovleniya-stalnyh-detaley/viewer">Ссылка </a></p>
      <p>А.А. Афанасьев, профессор, д.т.н., А.А. Стативко, доцент, к.т.н., Белгородский государственный технический университет имени В.Г. Шухова, г. Белгород, Россия  </p>
      <p>РАЗРАБОТКА РАЦИОНАЛЬНЫХ ТЕХНОЛОГИЧЕСКИХ СХЕМ УПРОЧНЕНИЯ И ВОССТАНОВЛЕНИЯ СТАЛЬНЫХ ДЕТАЛЕЙ </p>
      <p>Представлены результаты разработанной технологической схемы восстановления изношенной поверхности стальной детали оригинальным методом - обвивания шейки вала пластиной с последующими процессами достижения требуемой точности и упрочнения. </p>
      <p>Ключевые слова: восстановление поверхности, точечная сварка, ремонтный элемент, упрочнение поверхности. </p>
      <p>6.	<a href="https://cyberleninka.ru/article/n/vosstanovlenie-raspredelitelnogo-vala-dizelnogo-dvigatelya/viewer">Ссылка </a></p>
      <p>Латыпов Рашит Абдулхакович, д.т.н., профессор, Московский государственный машиностроительный университет, Агеев Евгений Викторович, д.т.н., профессор, Юго-Западный государственный университет, г. Курск, Латыпова Гюльнара Рашитовна, ст. преподаватель, Московский государственный машиностроительный университет</p>
      <p>ВОССТАНОВЛЕНИЕ РАСПРЕДЕЛИТЕЛЬНОГО ВАЛА ДИЗЕЛЬНОГО ДВИГАТЕЛЯ </p>
      <p>Предложена комплексная технология восстановления распределительного вала дизельного двигателя Raba-MAN, в соответствие с которой опорные шейки восстанавливают электроконтактной приваркой ленты через промежуточный слой из порошкового материала, а кулачки - элек- тродуговой наплавкой полым электродом в стандартной обмазке, содержащим порошок с включением наноразмерных частиц, полученных электроэррозионным диспергированием отходов твердого сплава ВК8.  </p>
      <p>Ключевые слова: распредвал, отходы твердых сплавов, электроэрозионное диспергирование, наноразмерные частицы, карбид вольфрама, восстановление, комплексная технология.  </p>
      <p>7.	<a href="https://cyberleninka.ru/article/n/povyshenie-dolgovechnosti-vosstanovlennyh-detaley-mashin-na-osnove-upravleniya-ostatochnymi-napryazheniyami/viewer">Ссылка </a></p>
      <p>А.Г. Игнатьев, А.А. Третьяков, Южно-Уральский государственный университет, г. Челябинск, Россия, 2ООО «ДСТ-Урал», г. Челябинск, Россия </p>
      <p>ПОВЫШЕНИЕ ДОЛГОВЕЧНОСТИ ВОССТАНОВЛЕННЫХ ДЕТАЛЕЙ МАШИН НА ОСНОВЕ УПРАВЛЕНИЯ ОСТАТОЧНЫМИ НАПРЯЖЕНИЯМИ </p>
      <p>Восстановление деталей обеспечивает повторное и неоднократное использование до 70 % изношенных деталей. </p>
	  <p>Восстановление деталей является экономически целесообраз-ным, себестоимость восстановления обычно не превышает 30 % стоимости новых деталей. </p>
	  <p>Однако использование большинства методов и технологий восстановления деталей приво-дит к снижению их долговечности в сравнении с новыми. </p>
	  <p>Для высоконагруженных валов фактором, определяющим их долговечность, является сопротивление усталости. </p>
	  <p>Первостепенным фактором, влияющим на усталостную прочность детали, является состояние поверхностного слоя. </p>
	  <p>Доминирующее значение в повышении сопротивления усталости восстановленных деталей принадлежит физико-механическим свойствам поверхностного слоя, упрочнению и остаточным напряжениям. </p>
	  <p>В статье рассмотрена технология восстановления деталей с использованием электроконтактной приварки металлической ленты. Получены данные о поверхностных остаточных напряжениях, возникающих в результате приварки покрытия. </p>
	  <p>Результаты измерений показали высокую нагруженность поверхностного слоя. Рассмотрены варианты снижения остаточных напряжений в восстановленных деталях применением поверхностного пла-стического деформирования и электроконтактного упрочнения. Для повышения долговечности деталей, восстановленных электроконтактной приваркой металлической ленты, рекомендовано применение электроконтактного упрочнения. Применение этого способа позволяет повысить предел выносливости восстановленных деталей в 1,5-2,5 раза. </p>
      <p>Ключевые слова: восстановление деталей, долговечность, предел выносливости, остаточные напряжения, поверхностное пластическое деформирование, электроконтактное упрочнение. </p>
      <p>8.	<a href="https://www.bstu.by/uploads/attachments/NIRS/%D0%92%D0%BE%D1%81%D1%81%D1%82%D0%B0%D0%BD%D0%BE%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D0%B5%20%D0%B4%D0%B5%D1%82%D0%B0%D0%BB%D0%B5%D0%B9%20%D0%BC%D0%B0%D1%88%D0%B8%D0%BD%20%D0%B8%20%D0%BC%D0%B5%D1%85%D0%B0%D0%BD%D0%B8%D0%B7%D0%BC%D0%BE%D0%B2%20%D0%BF%D0%BB%D0%B0%D1%81%D1%82%D0%B8%D1%87%D0%B5%D1%81%D0%BA%D0%B8%D0%BC%20%D0%BC%D0%BE%D0%B4%D0%B5%D0%BB%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D0%B5%D0%BC.pdf ">Ссылка </a></p>
      <p>Парфиевич А. Н. и Сокол В.А., ст. преподаватели каф. «Машиностроения и эксплуатации автомобилей» </p>
      <p>ВОССТАНОВЛЕНИЕ ДЕТАЛЕЙ МАШИН И МЕХАНИЗМОВ ПЛАСТИЧЕСКИМ ДЕФОРМИРОВАНИЕМ    </p>
      <p>Приведены основные принципы восстановления деталей пластическим деформированием, предложены конструкции специальных приспособлений для выполнения такого восстановления. </p>
	  <p>Ключевые слова: восстановаление, детали, машины </p>
      <p>9.	<a href="http://elib.psu.by:8080/bitstream/123456789/2103/1/Ivanov_Kastrjuk_2010-8-p2.pdf ">Ссылка </a></p>
      <p>Д-р техн. наук, проф. В.П. ИВАНОВ, канд. техн. наук, доц. А.П. КАСТРЮК (Полоцкий государственный университет) </p>
      <p>НОВАЯ КОНЦЕПЦИЯ ВОССТАНОВЛЕНИЯ ДЕТАЛЕЙ   </p>
      <p>Рассматривается новая концепция восстановления деталей – разработка модульных процессов восстановления деталей, повышающих эффективность ремонтно-восстановительного производства. </p>
	  <p>Определены геометрические и технологические модули восстанавливаемых деталей на основании классификации их элементов. Приведено содержание технологических модулей, обеспечивающих восстановление геометрических параметров и эксплуатационных свойств конструктивных элементов деталей. Показан состав технологического процесса восстановления детали из технологических модулей и обоснована эффективность предложенной концепции. Модульное построение процессов восстановления деталей – эффективное направление их технологической унификации. В составе технологической подготовки восстановительного производства оно обеспечивает нормативный уровень качества деталей с наименьшими затратами и трудоемкостью. </p>
      <p>Ключевые слова: восстановление, детали.  </p>
      <p>10. <a href="https://sat.bntu.by/jour/article/view/896/853 ">Ссылка </a></p>
      <p>В. П. Иванов, Полоцкий государственный университет, Новополоцк, Беларусь, Доктор технических наук, профессор </p>
      <p>ВЫБОР СПОСОБА ВОССТАНОВЛЕНИЯ ДЕТАЛЕЙ  </p>
      <p>Даны определения процесса и способа восстановления деталей с анализом известных методов их выбора. Определены геометрические параметры и эксплуатационные свойства, которые должны быть обеспечены при восстановлении деталей. </p>
	  <p>Усовершенствован выбор способа восстановления детали, позволяющий синтезировать оптимальный процесс этого восстановления по критерию расхода производственных ресурсов с учетом ограничений по качеству, производительности и безопасности. Обоснованы мероприятия, удовлетворяющие установленным ограничениям. Указана направленность технических решений, обеспечивающих полное использование остаточной долговечности деталей ремонтного фонда за счет применения без пропусков всех ремонтных размеров заготовок с уточнением их значений, равномерного снятия припуска при обработке заготовок резанием при оптимальном базировании, использования процессов нанесения покрытий только в технически обоснованных случаях, применения правки с термическим фиксированием ее результатов или всесторонним сжатием деформируемых элементов. Предложено ограничить число капитальных ремонтов агрегатов вместе с восстановлением базовых и основных деталей двумя ремонтами за весь их срок службы. Число наплавок шеек валов необходимо ограничить одной наплавкой в течение жизненного цикла детали с целью сохранения их длины в установленных пределах. Рекомендовано расширение области применения объемного пластического деформирования материала в виде термопластической раздачи или обжатия ремонтных заготовок класса «тела вращения с отверстиями», обеспечивающего припуск на обработку наружных и внутренних поверхностей под номинальные размеры без нанесения покрытий. Установлена структура материала покрытия с мелкодисперсными включениями карбидов или нитридов металлов и преимущественной ориентацией структурных составляющих перпендикулярно восстанавливаемой поверхности под влиянием отвода теплоты, которая в результате поверхностного пластического деформирования ориентирует оси волокон тангенциально в направлении относительного скольжения. Это препятствует росту усталостных радиально ориентированных трещин. </p>
      <p>Ключевые слова: деталь, восстановление, остаточная долговечность, оптимизация, параметры, ограничения. </p></td>
    </tr>
  </tbody>
</table>
</body>
</html>
