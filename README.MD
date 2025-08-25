# BCDenalClub.
## Робота із сайтом.
Для додавання/змін продуктів потрібно попрацювати із розділом відповідного продукту на сайті.  
Для початку роботи потрібно залогінітися на сайті та перейти на сторінку продукту.  
Для внесення змін на сторінці необхідно перейти в розділ **"Edit with Elementor"**  
<img src = "img/bcdental01.png" width = "1000">  
Для зміни даних щодо показників продукту (дати, час, тощо) необхідно виділити відповідний блок праворуч (1) і внести зміни у блоці (2), який відкриється ліворуч.  
<img src = "img/bcdental02.png" width = "1000">  

Плагін **Elementor** дозволяє визначати дії, які відбуваються при відправці форми. Передивитися ці дії модна в розділі **Actions after submit**, який знаходиться праворуч.  
<img src = "img/bcdental03.png" width = "1000">  

### Redirect

Після того, як користувач відправляє форму за логікою процесу він має попадати на сторінку оплати відповідного курсу. Для цього використоується розділ **Redirect**. Для того, щоб в платіжній сторінці був заповнений електронна поштова адреса така сама, як і та, яка введена при відправці пошти при редіректі прописуємо в якості GET-параметру **prefiled_email** зі значенням - шорт код, що відповідає полю введення електронної поштової адреси.  

<img src = "img/bcdental04.png" width = "1000">  

Уточнити шорт-код можна у розділі, який відповідає форму відправки даних.  

<img src = "img/bcdental05.png" width = "1000">  

### Site+MailChimp
Якщо додається новий продукт, то для нього потрібно створити новий тег. Це робиться в інтерфейсі сервісу **MailChimp**.
<img src = "img/bcdental07.png" width = "1000">  


Плагін **Elementor** дозволяє в якості події після відправки форми виконати дію щодо прикріплення певного тегу для певного email в сервісі **MailChimp**.
Для цього у блоці відповідної дії треба позначити тег, який треба прікріпити до користувача, що заповнуює форму.  При цьому, зв'язати поля форми для відправки даних та поля MailChimp та з'єднати сайт та відповідний обліковий запис MailChimp (робиться один раз, на цьому скріншоті не позначено).  

<img src = "img/bcdental06.png" width = "1000">  

### MailChimp. Lead reminder.
Для того, щоб реалізувати ланцюг нагадування клієнту, щодо оплати (якщо він заповнив форму і не оплатив впродовж 1 години). Ми використовуємо **MailChip Automation**.

<img src = "img/bcdental08.png" width = "1000">  

Для створення нового flow ми можемо використати існуючий (скопіювавши його).

<img src = "img/bcdental09.png" width = "1000">  

Або ж створити новий:  

<img src = "img/bcdental11.png" width = "1000">  

В flow є такі елементи як тег, при якому запускається automation (1), час, який проходить до перевірки, чи змінився тег на той, що відповідає покупці (2), перевірка, яи є у користувача тег, який відповідає покупці (3), повідомлення, що відправляється користувачеві, який не купив за відведений термін (4).

<img src = "img/bcdental12.png" width = "1000">  

Клієнт періодично створює повідомлення окремо. Їх неможливо перенести в automation автоматично, тому для їх переносу, як інструмент, є створення шаблону із такого повідомлення: 
<img src = "img/bcdental13.png" width = "1000">   
<img src = "img/bcdental14.png" width = "1000">   
<img src = "img/bcdental15.png" width = "1000">   

<img src = "img/bcdental16.png" width = "1000">   
<img src = "img/bcdental17.png" width = "1000">   
<img src = "img/bcdental18.png" width = "1000">   
<img src = "img/bcdental19.png" width = "1000">   
<img src = "img/bcdental20.png" width = "1000">   
<img src = "img/bcdental21.png" width = "1000">   
<img src = "img/bcdental22.png" width = "1000">   
<img src = "img/bcdental23.png" width = "1000">   
<img src = "img/bcdental24.png" width = "1000">   
<img src = "img/bcdental25.png" width = "1000">   
<img src = "img/bcdental26.png" width = "1000">   
<img src = "img/bcdental27.png" width = "1000">   
<img src = "img/bcdental28.png" width = "1000">   
<img src = "img/bcdental29.png" width = "1000">   
<img src = "img/bcdental30.png" width = "1000">   


### MailChimp. Participant confirmation.
Другий тип **MailChimp Automation** - це підтвердження оплати. В рамках логіги MailChimp - це відправлення повідомлення з підтвердження оплати при застосуванні тегу participant до користувача.  
Для створення таких Automation можна скопіювати існуючий Automation, або створити новий з нуля.

<img src = "img/bcdental37.png" width = "1000">  
<img src = "img/bcdental38.png" width = "1000">  
<img src = "img/bcdental39.png" width = "1000">  
<img src = "img/bcdental40.png" width = "1000">  
<img src = "img/bcdental41.png" width = "1000">  
<img src = "img/bcdental42.png" width = "1000">  
<img src = "img/bcdental43.png" width = "1000">  
<img src = "img/bcdental44.png" width = "1000">  
<img src = "img/bcdental45.png" width = "1000">  
<img src = "img/bcdental46.png" width = "1000">  
<img src = "img/bcdental47.png" width = "1000">  
<img src = "img/bcdental48.png" width = "1000">  
<img src = "img/bcdental49.png" width = "1000">  
<img src = "img/bcdental50.png" width = "1000">  
<img src = "img/bcdental51.png" width = "1000">  
<img src = "img/bcdental52.png" width = "1000">  
<img src = "img/bcdental53.png" width = "1000">  
<img src = "img/bcdental54.png" width = "1000">  
<img src = "img/bcdental55.png" width = "1000">  
<img src = "img/bcdental56.png" width = "1000">  

## Zapier
Після створення Automation для **Lead** та **Participant** тегів необхідно налаштувати **Zapier-automation**.  
Для цього зайдемо до облікового запису **Zapier**.  
Обираємо Zap, який відповідає продукту, із котрим ми працюємо:  
<img src = "img/bcdental57.png" width = "1000">  

Перевіряємо відповідність платіжного посилання.  
<img src = "img/bcdental58.png" width = "1000">  
<img src = "img/bcdental59.png" width = "1000">  

Перевіряємо відповіність групи (1), до якої додаємо користувача за умови, що він оплатив. Також перевіряємо, щоб код користувача передавася до DrivEd як customer id (2)

<img src = "img/bcdental60.png" width = "1000">  

Перевіряємо, щоб знімався правильни тег (Lead) 
<img src = "img/bcdental61.png" width = "1000">  
Даний тег має бути ідентичним тому, який надається користувачеві при заповненні ним форми на сторінці сайту відповідного продукту.  
<img src = "img/bcdental61_a.png" width = "1000">  

Перевіряємо тег, що відповівідає покупці продукту (participant)  
<img src = "img/bcdental62.png" width = "1000">  


Якщо користувач, що купив відповідний продукт не є преміум (немає одного з наступних тегів: **Premium Membership dentalcorp**, **Premium Membership**, **PREMIUM MEMBER $395**, **PREMIUM MEMBER $195**), то ви надаємо користувачеві тег Basic Membership, який дозволяє отримувати базову розсилку.  
Для цього в блоці **7**, первіряємо чи є наведені вище теги серед тегів, які є у користувача. В блоці **8** перевіряємо, чи знайшлося повертає блок **7** правду або брехню. Якщо блок **7** повертає брехню (користувач не є преміум), то блок **8** дозволяє виконати блок **9**, який, відповідно, надає користувачеві тег **Basic membership.**
<img src = "img/bcdental63.png" width = "1000">  


