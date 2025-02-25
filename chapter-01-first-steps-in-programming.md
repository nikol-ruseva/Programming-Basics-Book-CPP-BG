# Глава 1. Първи стъпки в програмирането

В тази глава ще разберем **какво е програмирането** в неговата същина. Ще се запознаем с идеята за **програмни езици** и ще разгледаме **средите за разработка на софтуер** (IDE) и как да работим с тях, в частност с **Visual Studio**. Ще напишем и изпълним **първата си програма** на програмния език **C++**, а след това ще се упражним с няколко задачи: ще създадем конзолни програми. Ще се научим как да проверяваме за коректност решенията на задачите от тази книга в **Judge системата на СофтУни** и накрая ще се запознаем с типичните грешки, които често се допускат при писането на код и как да се предпазим от тях.

## Видео

<div class="video-player">
  Гледайте видеоурок по тази глава тук: <a target="_blank"
  href="https://www.youtube.com/watch?v=CYPURYobOT8">
  https://www.youtube.com/watch?v=CYPURYobOT8</a>.
</div>

## Какво означава "да програмираме"?

**Да програмираме** означава да даваме команди на компютъра какво да прави, например "*да изсвири някакъв звук*", "*да отпечата нещо на екрана*" или "*да умножи две числа*". Когато командите са няколко една след друга, те се наричат **компютърна програма**. Текстът на компютърните програми се нарича **програмен код** (или **сорс код** или за по-кратко **код**).

### Компютърни програми

**Компютърните програми** представляват **поредица от команди**, които се изписват на предварително избран **език за програмиране**, например C++, Java, JavaScript, Python, Ruby, PHP, C, C#, Swift, Go или друг. За да пишем команди, трябва да знаем **синтаксиса и семантиката на езика**, с който ще работим, в нашия случай **C++**. Затова ще се запознаем със синтаксиса и семантиката на езика C++ и с програмирането като цяло в настоящата книга, изучавайки стъпка по стъпка писането на код, от по-простите към по-сложните програмни конструкции.

### Алгоритми

Компютърните програми обикновено изпълняват някакъв алгоритъм. **Алгоритмите** са последователност от стъпки, необходими, за да се свърши определена работа и да се постигне някакъв очакван резултат, нещо като "рецепта". Например, ако пържим яйца, ние изпълняваме някаква рецепта (алгоритъм): загряваме мазнина в някакъв съд, чупим яйцата, изчакваме докато се изпържат, отместваме от огъня. Аналогично, в програмирането **компютърните програми изпълняват алгоритми**: поредица от команди, необходими, за да се свърши определена работа. Например, за да се подредят поредица от числа в нарастващ ред, е необходим алгоритъм, примерно да се намери най-малкото число и да се отпечата, от останалите числа да се намери отново най-малкото число и да се отпечата и това се повтаря, докато числата свършат.

За удобство при създаването на програми, за писане на програмен код (команди), за изпълнение на програмите и за други операции, свързани с програмирането, ни е необходима и **среда за разработка**, например Visual Studio.

### Езици за програмиране, компилатори, интерпретатори и среди за разработка

**Езикът за програмиране** е изкуствен език (синтаксис за изразяване), предназначен за **задаване на команди**, които искаме компютъра да прочете, обработи и изпълни. Чрез езиците за програмиране пишем поредици от команди (**програми**), които **задават какво да прави компютъра**. Изпълнението на компютърните програми може да се реализира с **компилатор** или с **интерпретатор**.

**Компилаторът** превежда кода от програмен език на **машинен код**, като за всяка от конструкциите (командите) в кода избира подходящ, предварително подготвен фрагмент от машинен код, като междувременно **проверява за грешки текста на програмата**. Заедно компилираните фрагменти съставят програмата в машинен код, както я очаква микропроцесорът на компютъра. След като е компилирана програмата, тя може да бъде директно изпълнена от микропроцесора в кооперация с операционната система. При компилируемите езици за програмиране **компилирането на програмата** се извършва задължително преди нейното изпълнение и по време на компилация се откриват синтактичните грешки (грешно зададени команди). С компилатор работят езици като C++, C#, Java, Swift и Go.

Някои езици за програмиране не използват компилатор, а се **интерпретират директно** от специализиран софтуер, наречен "интерпретатор". **Интерпретаторът** е "**програма за изпълняване на програми**", написани на някакъв програмен език. Той изпълнява командите на програмата една след друга, като разбира не само от единични команди и поредици от команди, но и от другите езикови конструкции (проверки, повторения, функции и т.н.). Езици като PHP, Python и JavaScript работят с интерпретатор и се изпълняват без да се компилират. Поради липса на предварителна компилация, при интерпретируемите езици **грешките се откриват по време на изпълнение**, след като програмата започне да работи, а не предварително.

**Средата за програмиране** (Integrated Development Environment - **IDE**, интегрирана среда за разработка) е съвкупност от традиционни инструменти за разработване на софтуерни приложения. В средата за разработка пишем код, компилираме и изпълняваме програмите. Средите за разработка интегрират в себе си **текстов редактор** за писане на кода, **език за програмиране**, **компилатор или интерпретатор** и **среда за изпълнение** на програмите, **дебъгер** за проследяване на програмата и търсене на грешки, **инструменти за дизайн на потребителски интерфейс** и други инструменти и добавки.

**Средите за програмиране** са удобни, защото интегрират всичко необходимо за разработката на програмата, без да се напуска средата. Ако не ползваме среда за разработка, ще трябва да пишем кода в текстов редактор, да го компилираме с команда от конзолата, да го изпълняваме с друга команда от конзолата и да пишем още допълнителни команди, когато се налага, и това ще ни губи време. Затова повечето програмисти ползват IDE в ежедневната си работа.

За програмиране на **езика C++** най-често се ползва средата за разработка **Visual Studio**, която се разработва и разпространява безплатно от Microsoft и може да се изтегли от: https://www.visualstudio.com/downloads. Друга разпространена среда за разработка е **Code::Blocks** (https://www.codeblocks.org/downloads). В настоящата книга ще използваме средата за разработка **Visual Studio**.

### Езици от ниско и високо ниво, среди за изпълнение (Runtime Environments)

Програмата в своята същност е **набор от инструкции**, които карат компютъра да свърши определена задача. Те се въвеждат от програмиста и се **изпълняват безусловно от машината**.

Съществуват различни видове **езици за програмиране**. С езиците от най-ниско ниво могат да бъдат написани **самите инструкции**, които **управляват процесора**, например с езика "**assembler**". С езици от малко по-високо ниво като **C** и **C++** могат да бъдат създадени операционна система, драйвери за управление на хардуера (например драйвер за видеокарта), уеб браузъри, компилатори, двигатели за графика и игри (game engines) и други системни компоненти и програми. С езици от още по-високо ниво като **C#**, **Python** и **JavaScript** се създават приложни програми, например програма за четене на поща или чат програма.

**Езиците от ниско ниво** управляват директно хардуера и изискват много усилия и огромен брой команди, за да свършат единица работа. **Езиците от по-високо ниво** изискват по-малко код за единица работа, но нямат директен достъп до хардуера. На тях се разработва приложен софтуер, например уеб приложения и мобилни приложения.

Болшинството софтуер, който използваме ежедневно, като музикален плеър, видеоплеър, GPS програма и т.н., се пише на **езици за приложно програмиране**, които са от високо ниво, като C++, Java, Python, C#, JavaScript, PHP и др.

**C++ е компилируем език**, а това означава, че пишем команди, които се компилират до машинен код преди да се изпълнят. Именно тези команди, чрез помощна програма (компилатор), се преобразуват във файл, който може да се изпълнява (executable). За да пишем на език като **C++** ни трябва текстов редактор или среда за разработка.

### Компютърни програми - компилация и изпълнение

Както вече споменахме, програмата е **последователност от команди**, иначе казано тя описва поредица от пресмятания, проверки, повторения и всякакви подобни операции, които целят постигане на някакъв резултат.

Програмата се пише в текстов формат, а самият текст на програмата се нарича **сорс код** (source code). Той се компилира до **изпълним файл** (например **`Program.cpp`** се компилира до **`Program.exe`**).

Процесът на **компилация** на кода преди изпълнение е присъщ само за компилируеми езици като C++, Java, C# и др. При **скриптови и интерпретеруеми езици**, като JavaScript, Python и PHP, сорс кодът се изпълнява **постъпково** от интерпретатор.

### Компютърни програми – примери

Да започнем с много прост пример за кратка C++ програма.

#### Пример: програма, която отпечатва даден текст

Нашата първа програма ще е единична C++ команда, която отпечатва текста "**Hello**":

```cpp
#include <iostream>
using namespace std;

int main() {
    cout << "Hello";
    
    return 0;
}
```
Може да тествате примера онлайн: https://repl.it/@nakov/CPlusPlus-Hello.

След малко ще разберем как можем да изпълним тази команда и да видим отпечатания текст, но засега нека само разгледаме какво представляват командите в програмирането. Да се запознаем с още няколко примера.

#### Пример: програма, която отпечатва английската азбуката

Можем да усложним предходната програма, като зададем за изпълнение повтарящи се в цикъл команди за извеждане на текст:

```cpp
for (char ch = 'A'; ch <= 'Z'; ch++) {
    cout << ch << endl;
}
```
Може да тествате примера онлайн: https://repl.it/@vncpetrov/EnglishAlphabet.

В горния пример караме компютъра да отпечатва един след друг, на нови редове, много символи, започвайки от А и приключвайки с Z. Резултатът от програмата е отпечатване на цялата английска азбука.

Как работят повторенията (циклите) в програмирането ще научим в **глава "[Повторения (цикли)](chapter-05-loops.md)"**, но засега нека приемем, че просто повтаряме някаква команда много пъти.

#### Пример: програма, която конвертира от левове в евро

Да разгледаме още една проста програма, която прочита от потребителя някаква сума в лева (цяло число), конвертира я в евро (като я разделя на курса на еврото) и отпечатва получения резултат. Това е програма от 4 поредни команди:

```cpp
double leva;
cin >> leva;
double euro = leva / 1.95583;
cout << euro << endl;
```
Може да тествате примера онлайн: https://repl.it/@vncpetrov/LevaToEuro.

Разгледахме **три примера за компютърни програми**: единична команда, серия команди в цикъл и поредица от 4 команди. Нека сега преминем към по-интересното: как можем да пишем собствени програми на **C++** и как можем да ги компилираме и изпълняваме?

## Как да напишем конзолна програма?

Нека преминем през **стъпките за създаване и изпълнение на компютърна програма**, която чете и пише своите данни от и на текстова конзола (прозорец за въвеждане и извеждане на текст). Такива програми се наричат "**конзолни**". Преди това, обаче, трябва първо да си **инсталираме и подготвим средата за разработка**, в която ще пишем и изпълняваме C++ програмите от тази книга и упражненията към нея.

## Среда за разработка (IDE)

Както вече стана дума, за да програмираме ни е нужна **среда за разработка** - **Integrated Development Environment** (IDE). Това всъщност е редактор за програми, в който пишем програмния код и можем да го изпълняваме, да виждаме грешките, да ги поправяме и да стартираме програмата отново.
 - За програмиране на C++ използваме средата **Visual Studio** за операционната система Windows и **Eclipse** за Linux или Mac OS X.
 - Ако програмираме на Java, подходящи са средите **IntelliJ IDEA**, **Eclipse** или **NetBeans**.
 - Ако ще пишем на Python, можем да използваме средата **PyCharm**.

### Инсталация на Visual Studio Community

Започваме с инсталацията на интегрираната среда **Microsoft Visual Studio Community** (версия 2017, актуална към януари 2019 г.).

**Community** версията на Visual Studio (VS) се разпространява безплатно от Microsoft и може да бъде изтеглена от: [https://www.visualstudio.com/vs/community](https://www.visualstudio.com/vs/community). Инсталацията е типичната за Windows с [**Next**], [**Next**] и [**Finish**], но е важно да включим компонентът за "**Desktop development with C++**". Не е необходимо да променяме останалите настройки за инсталация.

В следващите редове са описани подробно **стъпките за инсталация на Visual Studio** (версия Community 2017). След като свалим инсталационния файл и го стартираме, се появява следният екран:

![](/assets/chapter-1-images/00.visual-studio-01.png)

Натискаме бутона [**Continue**], след което ще видим прозореца долу:

![](/assets/chapter-1-images/00.visual-studio-02.png)

Зарежда се прозорец с инсталационния панел на Visual Studio. Слагаме отметка на [**Desktop development with C++**], след което натискаме бутона [**Install**]:

![](/assets/chapter-1-images/00.visual-studio-03.png)

Започва инсталацията на Visual Studio и ще се появи екран като този по-долу:

![](/assets/chapter-1-images/00.visual-studio-05.png)

След като Visual Studio се инсталира, ще иска да рестарираме компютъра, преди да го отворим. Можем да натиснем бутона [**Not now**], ако не искаме да рестартираме веднага компютъра си, но трябва задължително да го направим преди да ползваме **Visual Studio**. Ако сме готови веднага да рестартираме, натискаме бутона [**Restart**]. След това компютърът ще се рестартира. Когато се включи отново, пускаме **Visual Studio**. Ако инсталираме по-стара или различна версия е възможно да не се изисква рестартиране. Тогава само трябва да натиснем бутона [**Launch**], за да стартираме **Visual Studio**:

![](/assets/chapter-1-images/00.visual-studio-06.png)

След **старта на VS** излиза екран като този по-долу. От него можем да изберем дали да влезем с Microsoft профила си. За момента избираме да работим без да сме се логнали с Microsoft акаунта си, затова избираме опцията [**Not now, maybe later.**]. На по-късен етап, ако имате такъв акаунт, можете да се логнете, а ако нямате и срещате затруднения със създаването му, винаги можете да пишете във форума на SoftUni: [https://softuni.bg/forum](https://softuni.bg/forum):

![](/assets/chapter-1-images/00.visual-studio-07.png)

Следващата стъпка е да изберем **цветовата тема**, с която да се визуализира Visual Studio. Тук изборът е изцяло според предпочитанията на потребителя, като няма значение коя опция ще бъде избрана:

![](/assets/chapter-1-images/00.visual-studio-08.png)

Натискаме бутона [**Start Visual Studio**] и се зарежда началния изглед на Visual Studio Community:

![](/assets/chapter-1-images/00.visual-studio-09.png)

Това е всичко. Готови сме за работа с Visual Studio.

### По-стари версии на Visual Studio

Можем да използваме и по-стари версии на Visual Studio (например версия 2015 или 2013 или дори 2010 или 2005), но **не е препоръчително**, тъй като в тях не се съдържат някои от по-новите възможности за разработка и не е сигурно дали всички примери от книгата ще тръгнат.

### Онлайн среди за разработка

Съществуват и **алтернативни среди за разработка онлайн**, директно във вашия уеб браузър. Тези среди не са много удобни, но ако нямате друга възможност, може да стартирате обучението си с тях и да си инсталирате Visual Studio на по-късен етап. Ето някои линкове:
* За езика C++ можем да използваме: [http://cpp.sh](http://cpp.sh)
* За езика C# сайтът **.NET Fiddle** позволява писане на код и изпълнението му онлайн: [https://dotnetfiddle.net](https://dotnetfiddle.net).
* За Java можем да използваме следното онлайн Java IDE: [https://www.compilejava.net](https://www.compilejava.net).
* За JavaScript можем да пишем JS код директно в конзолата на даден браузър с натискане на **[F12]**.

### Проектни решения и проекти във Visual Studio

Преди да започнем да работим с Visual Studio е нужно да се запознаем с понятията **Visual Studio Solution** и **Visual Studio Project**, които са неизменна част от него.

**Visual Studio Project** представлява "проектът", върху който работим. В началото това ще са нашите конзолни програми, които ще се научим да пишем с помощта на настоящата книга, ресурсите към нея и в курса Programming Basics в SoftUni. При по-задълбочено изучаване и с времето и практиката, тези проекти ще преминат в апликации, игри и други разработки. Проектът във VS **логически групира множество файлове**, изграждащи дадено приложение или компонент. Един **C++ проект** съдържа един или няколко **C++ сорс файла**, конфигурационни файлове и други ресурси. Във всеки C++ сорс файл има една или повече **дефиниции на типове** (класове или други дефиниции). В **класовете** има **методи** (действия), а те се състоят от **поредици от команди**. Изглежда сложно, но при големи проекти такава структура е много удобна и позволява добра организация на работните файлове.

**Visual Studio Solution** представлява контейнер (работно решение), в който **логически са обединени няколко проекта**. Целта на обединението на тези VS Projects е да има възможност кодът от който и да е от проектите да си взаимодейства с кода на останалите VS проекти, за да може приложението да работи коректно. Когато софтуерният продукт или услуга, който разработваме, е голям, той се изгражда като **VS Solution**, а този Solution се разделя на **проекти** (VS Projects) и във всеки проект има **папки със сорс файлове**. Такава йерархична организация е много удобна при по-сериозни проекти (да кажем над 50 000 реда код).

За **малки проекти** VS Solutions и VS Projects повече **усложняват работата**, отколкото помагат, но се свиква бързо.

## Пример: създаване на конзолна програма "Hello C++"

Да се върнем на нашата конзолна програма. Вече имаме Visual Studio и можем да го стартираме. След това създаваме нов конзолен проект: [**File**] &rarr; [**New**] &rarr; [**Project…**]:

![](/assets/chapter-1-images/01.Hello-c++-01.png)

Ще се отвори прозорец, който ще изглежда като картинка по-долу. Трябва да изберем [**Visual C++**] &rarr; [**Empty Project**]. След което задаваме **смислено име** на нашия проект, например **"HelloC++"**: 
![](/assets/chapter-1-images/01.Hello-c++-02.png)

Когато сме готови, натискаме бутона [**OK**] и Visual Studio ще създаде за нас VS Solution с един празен C++ проект в него:

![](/assets/chapter-1-images/01.Hello-c++-03.png)

За да добавим **празна C++ програма** в новосъздадения проект, трябва да изберем: [**Project**] &rarr; [**Add new item…**]:
![](/assets/chapter-1-images/01.Hello-c++-04.png)

След което ще се отвори прозорец, в който трябва да изберем [**Visual C++**] &rarr; [**C++ file(.cpp)**]. Задаваме **смислено име** на нашата програма, например **`HelloC++.cpp`**. Ако забравим да напишем **.cpp** разширението, Visual Studio ще го добави:

![](/assets/chapter-1-images/01.Hello-c++-05.png)

Когато сме готови, натискаме бутона [**Add**] и ще се отвори **празна C++ програма**, където ще можем да пишем код:

![](/assets/chapter-1-images/01.Hello-c++-06.png)

### Писане на програмен код

За сега всяка наша програма трябва да започваме със следния код:

![](/assets/chapter-1-images/01.Hello-c++-07.png)

Също така за сега ще пишем командите само във функцията **`int main()`**, между отварящата и затварящата скоба **`{ }`**. Това е главната функция (действие), което се изпълнява при стартиране на една конзолна C++ програма. По-нататък в книгата, в глава **[Функции](chapter-10-functions.md)"**, ще се запознаем по-подборно какво представляват функциите и как можем да ги използваме. 

Натискаме [**Enter**] след **отварящата скоба** **`{`** и **започваме да пишем**. Кодът на програмата се пише **отместен навътре**, като това е част от оформянето на текста, за по-голямо удобство при повторен преглед и/или дебъгване. Пишем следната команда:

```cpp
cout << "Hello C++" << endl;
```
Може да тествате примера онлайн: https://repl.it/@vncpetrov/HelloCPP1.

Ето как трябва да изглежда нашата програма във Visual Studio:

![](/assets/chapter-1-images/01.Hello-c++-08.png)

Командата **`cout << "Hello C++" << endl;`** означава да изпълним отпечатване върху конзолата и да отпечатаме текстовото съобщение **`Hello C++`**, което трябва да оградим с кавички, за да поясним, че това е текст. **`endl`** означава нов ред, а **`cout << endl;`** означава отпечатване на нов ред. Тези команди могат да се напишат и на два реда:

```cpp
cout << "Hello C++";
cout << endl;
```
Може да тествате примера онлайн: https://repl.it/@vncpetrov/HelloCPP2.

В края на всяка команда на езика C++ се слага символът **`;`**. Tой указва, че командата свършва на това място (т.е. не продължава на следващия ред).

Редът **`#include<iostream>`** означава включи библиотеката **iostream**. Библиотеките са код, който е написан от някой друг и можем да използваме наготово. Например от библиотеката **iostream** използваме **`cin`** и **`cout`**. Има най-различни други библиотеки, също така можем и сами да си пишем библиотеки, но това не е предмет на настоящата книга.

Редът **`using namespace std;`** означава използвай namespace **`std`**. Какво е namespace? Представете си, че по даден проект работят много хора, сред които Пешо и Гошо. Пешо иска да си кръсти някоя променлива **`count`**, но и Гошо иска да използва променлива с име **`count`**. За компилатора тези две променливи ще означават едно и също, независимо дали Пешо или Гошо я използва. За да се реши този проблем, се използва **namespace**. Тогава Пешо ще си има namespace **`Peter`**, а Гошо ще си има namespace **`Geore`**. За да използва Пешо своята променлива **`count`**, ще напише **`Peter::count`**, а Гошо, за да използва своята променлива **`count`**, ще напише съответно **`George::count`**. Тогава вече компилаторът ще прави разлика между променливата **`count`** на Гошо и съответно на Пешо. Символите **`::`** означават да се вземе променливата, написана отдясно на **`::`**, от namespace-а, написан отляво на **`::`**. 

Има и готови namespaces, като например **std**. Съкращението **std** идва от **Standard Template Library** и конкретно от думата **standart**. Няколко библиотеки са обединени в namespace **std**. Т.е. за да използваме нещата от тях, трябва да пишем навсякъде **`std::…`**. Както вече казахме, редът **`using namespace std;`** означава използвай namespace **std**. Т.е. ако го напишем в програмата си, включваме всички неща от съответния namespace и няма нужда навсякъде да пишем **`std::…`**. Горният пример без този ред ще изглежда така:

![](/assets/chapter-1-images/01.Hello-c++-09.png)

За улеснение, в книгата ще използваме първия вариант с **`using namespace std;`**.

### Стартиране на програмата

За стартиране на програмата натискаме [**Ctrl + F5**]. Ако няма грешки, програмата ще се изпълни. Резултатът ще се изпише на конзолата (в черния прозорец):

![](/assets/chapter-1-images/01.Hello-c++-10.png)

Забележете, че стартираме с **[Ctrl + F5]**, а не само с **[F5]** или с бутона за стартиране във Visual Studio. Ако използваме **[F5]**, програмата ще се изпълни за кратко и веднага след това конзолата ще изчезне и няма да видим резултата.

Всъщност, изходът от програмата е следното текстово съобщение:

```cpp
Hello C++
```

Съобщението "**Press any key to continue …**" се изписва допълнително на най-долния ред на конзолата от Visual Studio след като програмата завърши изпълнението си, за да ни подкани да натиснем клавиш, за да затворим конзолата.

Възможно е **[Ctrl + F5]** да не работи и конзолата да се затваря веднага. За да оправим проблема, трябва да добавим следния ред код на реда **преди `return 0;`**:

```cpp
system("pause");
```

Кодът ни ще изглежда така:

![](/assets/chapter-1-images/01.Hello-c++-11.png)

Ако имаме този проблем, няма значение дали стартираме с **[Ctrl + F5]** или само с **[F5]**.

### Тестване на програмата в Judge системата

Тестването на задачите от тази книга е автоматизирано и се осъществява през Интернет, от сайта на **Judge системата**: [https://judge.softuni.org](https://judge.softuni.org). Оценяването на задачите се извършва на момента от системата. Всяка задача минава поредица от тестове, като всеки успешно преминат тест дава предвидените за него точки. Тестовете, които се подават на задачите, са скрити.

Горната програма може да тестваме тук: [https://judge.softuni.org/Contests/Practice/Index/1357#0](https://judge.softuni.org/Contests/Practice/Index/1357#0). Поставяме целия сорс код на програмата в черното поле и избираме **C++ code**, както е показано тук:

![](/assets/chapter-1-images/01.Hello-c++-12.png)

Изпращаме решението за оценяване с бутона [**Изпрати**] (или [**Submit**]). Системата връща резултат след няколко секунди в таблицата с изпратени решения. При необходимост може да натиснем бутона за обновяване на резултатите **[Refresh]**, който се намира в горната дясна част на таблицата с изпратени за проверка решения:

![](/assets/chapter-1-images/01.Hello-c++-13.png)

В таблицата с изпратените решения Judge системата ще покаже един от следните **възможни резултати**:
* **Брой точки** (между 0 и 100), когато предаденият код се компилира успешно (няма синтактични грешки) и може да бъде тестван.
  - При **вярно решение** всички тестове са маркирани в зелено и получаваме **100 точки**.
  - При **грешно решение** някои от тестовете са маркирани в червено и получаваме непълен брой точки или 0 точки.
* При грешна програма ще получим **съобщение за грешка** по време на компилация.

### Как да се регистрирам в SoftUni Judge?

Използваме идентификацията си (Username + Password) от сайта [softuni.bg](softuni.bg). Ако нямате СофтУни регистрация, направете си. Отнема само минутка - стандартна регистрация в Интернет сайт.

## Тествайте примерните програми

Сега, след като вече **знаете как да изпълнявате програми**, можете да тествате примерните програми по-горе. Позабавлявайте се, пробвайте да ги промените и да си поиграете с тях.

## Типични грешки в C++ програмите

**Липсата на точка и запетая** (**`;`**) в края на командите е един от вечните проблеми на начинаещия програмист. Пропускането на този знак води до **неправилно функциониране на програмата** или до **нейното неизпълнение** и **често проблемът остава незабелязан**. Ето примерен грешен код:

```cpp
#include <iostream>
using namespace std;

int main() {
    int x;
    cin >> x
    cout << x;
}
```

При опит за компилация, във Visual Studio ще се появи следният прозорец, който ни казва, че има проблем:

![](/assets/chapter-1-images/02.Errors-01.png)

Ако натиснем [**Yes**], ще се изпълни последната версия на програмата, която се е компилирала успешно. Ако обаче изберем [**No**], ще можем да видим списъка с грешки, който се намира в прозорец **Error List**, под кода на нашата програма:

![](/assets/chapter-1-images/02.Errors-02.png)

**Допълнителна точка и запетая** (**`;`**) също е проблем. Това също води до **неправилно функциониране на програмата** или до **нейното неизпълнение**. Пример за грешен код:

```cpp
#include <iostream>
using namespace std;

int main() ;
{
    int x;
    cin >> x
    cout << x;
}
```

Във Visual Studio ще се появи следната грешка:

![](/assets/chapter-1-images/02.Errors-03.png)

**Недекларирани променливи**. В следващия пример компилаторът не знае какво е **`x`**, защото първо трябва да се зададе тип на променливата. Програмата отново **няма да се изпълни**:

```cpp
#include <iostream>
using namespace std;

int main() {
    cin >> x;
    cout << x;
}
```

Във Visual Studio ще се появи следната грешка:

![](/assets/chapter-1-images/02.Errors-04.png)

Липсваща **кавичка** или **липса на отваряща или затваряща скоба (неправилен брой скоби)** също може да се окажат проблеми. Както и при точката и запетаята, така и тук проблемът води до **неправилно функциониране на програмата** или въобще до **нейното неизпълнение**. Този пропуск трудно се забелязва при по-обемен код. Ето пример за грешна програма:

```cpp
#include <iostream>
using namespace std;

int main()
    int x;
    cin >> x;
    cout << x;
}
```

Тази програма ще даде **грешка при опит за компилация** и стартиране и дори още преди това кодът ще бъде подчертан, за да се насочи вниманието на програмиста към грешката, която е допуснал (пропуснатата отваряща скоба). Тук списъкът от грешки ще е по-дълъг, което може да е малко объркващо в началото:

![](/assets/chapter-1-images/02.Errors-05.png)

## Какво научихме от тази глава?

На първо място научихме **какво е програмирането** - **задаване на команди, изписани на компютърен език**, които машината разбира и може да изпълни. Разбрахме още какво е **компютърна програма** - тя представлява **поредица от команди**, подредени една след друга. Запознахме се с **езика за програмиране C++** на базисно ниво и как **да създаваме прости конзолни програми** с Visual Studio. Проследихме и **структурата на програмния код в езика C++**, като например, че за сега ще задаваме командите в секцията **``int main()``** между **отварящата и затварящата къдрава скоба**. Видяхме как да печатаме с **`cout << … ;`** и как да стартираме програмата си с [**Ctrl + F5**]. Научихме се да тестваме кода си в **SoftUni Judge** системата и се запознахме с типични грешки в C++ програмите.

Добра работа! Да се захващаме с **упражненията**. Нали не сте забравили, че програмиране се учи с много писане на код и решаване на задачи? Да решим няколко задачи, за да затвърдим наученото.

## Упражнения: първи стъпки в коденето

Добре дошли в упражненията. Сега ще напишем няколко конзолни програми, с които ще направим още няколко първи стъпки в програмирането.

### Задача: програма “Expression”

Да се напише C++ програма, която **пресмята** и **отпечатва** стойността на следния числен израз:

<p align="center"> (3522 + 52353) * 23 - (2336 * 501 + 23432 - 6743) * 3 </p>

Забележка: **не е разрешено да се пресметне стойността предварително** (например с Windows Calculator).

#### Насоки и подсказки

Правим нов **C++ празен проект** с име "**Expression**".	Написваме си първоначалния код, **влизаме в тялото на int main()** между **`{`** и **`}`**. След това трябва да **напишем кода**, който да изчисли горния числен израз и да отпечата на конзолата стойността му. Пишем горния числов израз на мястото на многоточието в следната команда: **``cout << … ;``**:

![](/assets/chapter-1-images/03.Expression-01.png)

Стартираме програмата с [**Ctrl+F5**] и проверяваме дали резултатът е същия като на картинката:

![](/assets/chapter-1-images/03.Expression-02.png)

#### Тестване в Judge системата

Тествайте решението си тук: [https://judge.softuni.org/Contests/Practice/Index/1357#1](https://judge.softuni.org/Contests/Practice/Index/1357#1).

![](/assets/chapter-1-images/03.Expression-03.png)


### Задача: числата от 1 до 20

Да се напише C++ програма, която **отпечатва числата от 1 до 20** на отделни редове на конзолата.

#### Насоки и подсказки

Създаваме нов **C++ празен проект** с име "**Nums1To20**". В **`int main()`** функцията пишем 20 команди **``cout << … << endl;``**, всяка на отделен ред, за да отпечатаме числата от 1 до 20 едно след друго:

```cpp
cout << 1 << endl;
cout << 2 << endl;
…
```
Може да тествате примера онлайн: https://repl.it/@vncpetrov/Nums1To20.

По-досетливите от вас, сигурно се питат дали няма по-умен начин. Спокойно, има, но за него ще научим по-късно.

![](/assets/chapter-1-images/04.Numbers-1-to-20-01.png)

Сега **стартираме програмата** и поверяваме дали резултатът е какъвто се очаква да бъде:
```
1
2
…
20
```

#### Тестване в Judge системата

Тествайте решението си тук: [https://judge.softuni.org/Contests/Practice/Index/1357#2](https://judge.softuni.org/Contests/Practice/Index/1357#2).

Сега помислете дали може да напишем програмата по **по-умен начин**, така че да не повтаряме 20 пъти една и съща команда. Потърсете в Интернет информация за "**[for loop C++](https://www.google.bg/search?ei=c1M2XOj4Hq2ygwfi5abYCg&q=for+loop+C%2B%2B&oq=for+loop+C%2B%2B&gs_l=psy-ab.3..0i71l8.0.0..11731...0.0..0.0.0.......0......gws-wiz.xCpG9EXvoh4)**".

### Задача: триъгълник от 55 звездички

Да се напише C++ програма, която **отпечатва триъгълник от 55 звездички**, разположени на 10 реда:

```
*
**
***
****
*****
******
*******
********
*********
**********
```

#### Насоки и подсказки

Създаваме нов **C++ празен проект** с име "**TriangleOf55Stars**". В него трябва да напишем код, който печата триъгълника от звездички, например чрез 10 команди, като посочените по-долу:

```cpp
cout << "*" << endl;
cout << "**" << endl;
…
```
Може да тествате примера онлайн: https://repl.it/@vncpetrov/TriangleOf55Stars.

#### Тестване в Judge системата

Тествайте решението си тук: [https://judge.softuni.org/Contests/Practice/Index/1357#3](https://judge.softuni.org/Contests/Practice/Index/1357#3).

Опитайте да **подобрите решението**, така че да няма много повтарящи се команди. Може ли това да стане с **`for`** цикъл? Успяхте ли да намерите умно решение (например с цикъл) на предната задача? При тази задача може да се ползва нещо подобно, но малко по-сложно (два цикъла един в друг). Ако не успеете, няма проблем, ще учим цикли след няколко глави и ще си спомните за тази задача тогава.

### Задача: лице на правоъгълник

Да се напише C++ програма, която **прочита** от конзолата **две числа a и b**, **пресмята** и **отпечатва** лицето на правоъгълник със страни **a** и **b**. 

#### Примерен вход и изход

|   a   |   b   |  area  |
| ----- | ----- | ------ |
|   2   |   7   |   14   |
|   7   |   8   |   56   |
|   12  |   5   |   60   |

#### Насоки и подсказки

Правим нов **C++ празен проект**. За да **прочетем двете числа**, използваме следната команда команди:

```cpp
int a, b;
cin >> a >> b;
```
Може да тествате примера онлайн: https://repl.it/@vncpetrov/RectangleArea.

Остава да се допише програмата по-горе, за да пресмята лицето на правоъгълника и да го отпечата. Използвайте познатата ни вече команда **`cout << … ;`** и на мястото на многоточието напишете произведението на числата **a** и **b**. В програмирането умножението се извършва с оператора **`*`**.

![](/assets/chapter-1-images/05.Rectangle-area-01.png)

#### Тествайте решението си

Тествайте решението си с няколко примера. Трябва да получите резултат, подобен на този (въвеждаме 2 и 7 като вход и програмата отпечатва като резултат 14 - тяхното произведение):

```
2
7
14
```

#### Тестване в Judge системата

Тествайте решението си тук: [https://judge.softuni.org/Contests/Practice/Index/1357#4](https://judge.softuni.org/Contests/Practice/Index/1357#4).


### \* Задача: квадрат от звездички

Да се напише C++ програма, която **прочита** от конзолата **цяло положително число N** и **отпечатва** на конзолата **квадрат от N звездички**, като в примерите по-долу.

#### Примерен вход и изход

| Вход  |    Изход   	| Вход  |    Изход   	| Вход  |    Изход   	| 
|-----|-----------|-----|-----------|-----|----------|
|  3  	|<code>\*\*\*</code><br><code>\*&nbsp;\*</code><br><code>\*\*\*</code>|  4  |<code>\*\*\*\*</code><br><code>\*&nbsp;&nbsp;\*</code><br><code>\*&nbsp;&nbsp;\*</code><br><code>\*\*\*\*</code>| 5  	|<code>\*\*\*\*\*</code><br><code>\*&nbsp;&nbsp;&nbsp;\*</code><br><code>\*&nbsp;&nbsp;&nbsp;\*</code><br><code>\*&nbsp;&nbsp;&nbsp;\*</code><br><code>\*\*\*\*\*</code>|

#### Насоки и подсказки

Правим нов **C++ празен проект**. За да прочетем числото **N** (2 ≤ N ≤100), използваме следния код:

```cpp
int n;
cin >> n;
```
Може да тествате примера онлайн: https://repl.it/@vncpetrov/SquareOfStars.

Да се допише програмата по-горе, за да отпечатва квадрат, съставен от звездички. Може да се наложи да се използват **`for`** цикли. Потърсете информация в Интернет.

**Внимание**: тази задача е по-трудна от останалите и нарочно е дадена сега и е обозначена със звездичка, за да ви провокира да потърсите информация в Интернет. Това е едно от най-важните умения, което трябва да развивате докато учите програмирането: **да търсите информация в Интернет**. Това ще правите всеки ден, ако работите като програмисти, така че не се плашете, а се опитайте. Ако имате трудности, можете да потърсите помощ и в СофтУни форума: [https://softuni.bg/forum](https://softuni.bg/forum).

#### Тестване в Judge системата

Тествайте решението си тук: [https://judge.softuni.org/Contests/Practice/Index/1357#5](https://judge.softuni.org/Contests/Practice/Index/1357#5).

## Конзолни, графични и уеб приложения

При **конзолните приложения** (Console Applications), както и сами можете да се досетите, **всички операции** за четене на вход и печатане на изход се **извършват през конзолата**. Там се **въвеждат входните данни**, които се прочитат от приложението, там се **отпечатват и изходните данни** след или по време на изпълнение на програмата.

Докато конзолните приложения **ползват текстовата конзола**, уеб приложенията (Web Аpplications) **използват уеб-базиран потребителски интерфейс**. За да се **постигне тяхното изпълнение** са необходими две неща - **уеб сървър** и **уеб браузър**, като **браузърът** играе главната роля по **визуализация на данните и взаимодействието с потребителя**. Уеб приложенията са много по-приятни за потребителя, изглеждат визуално много по-добре, използват се мишка и докосване с пръст (при таблети и телефони), но зад всичко това стои програмирането. И затова **трябва да се научим да програмираме** и вече направихме първите си съвсем малки стъпки.

**Графичните (GUI) приложения** имат **визуален потребителски интерфейс**, директно върху вашия компютър или мобилно устройство, без да е необходим уеб браузър. Графичните приложения (настолни приложения или, иначе казано, desktop apps) **се състоят от един или повече графични прозореца**, в които се намират определени **контроли** (текстови полета, бутони, картинки, таблици и други), **служещи за диалог** с потребителя по по-интуитивен начин. Подобни са и мобилните приложения във вашия телефон и таблет: ползваме форми, текстови полета, бутони и други контроли и ги управляваме чрез програмен код. Нали затова се учим сега да пишем код: **кодът е навсякъде в разработката на софтуер**.

Страшно ли изглежда? **Не се плашете!** Имаме да извървим дълъг път, за да достигнем ниво на знания и умения, за да пишем свободно код на C++ в много по-големи и по-сложни програми. Ако не успеете да се справите, няма страшно, продължете спокойно напред. След време ще си спомняте с усмивка колко непонятен и вълнуващ е бил първият ви сблъсък с програмирането. Ако имате проблеми с примерите по-горе, **гледайте видеото** в началото на тази глава или питайте във **форума на СофтУни**: https://softuni.bg/forum. **Имате да учите още много**, но пък е интересно, нали?
