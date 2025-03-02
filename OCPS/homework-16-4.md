# Домашнее задание к занятию «Решение задач оперативного учёта. Часть 3»

## Цель задания

1. Закрепить полученные на лекции знания.
2. Научиться самостоятельно решать задачи оперативного учёта из экзамена «‎1С:Специалист по Платформе».

Эта практика позволит вам определить свои сильные и слабые стороны в решении задач оперативного учёта и пригодится для самостоятельной подготовки к экзамену.

## Чек-лист готовности к домашнему заданию

- скачать каркасную конфигурацию [файл new_carcass_8_3_17_1496.dt](https://github.com/Bofh82/onec-mid-homeworks/blob/main/OCPS/new_carcass_8_3_17_1496.dt),
- создать пустую информационную базу,
- загрузить в неё каркасную конфигурацию,
- просмотреть материал занятия.

## Инструкция к заданию

1. Решите описанную задачу в конфигураторе.
2. Протестируйте решение в пользовательском режиме.
3. Отправьте на проверку в личном кабинете Нетологии один файл выгрузки базы данных (.dt), содержащий решение задачи. Файл прикрепите в раздел «Решение» в практическом задании. Имя файла должно быть в формате «ФамилияИО_ОУ2.dt».

## Описание задачи

Необходимо создать интерфейс решения учебной задачи. В интерфейсе должно быть создано три раздела: «Главное», «Оперативный учёт», «Сервис». Панель навигации вместе с панелью действий на закладке «Оперативный учёт» должна обеспечивать доступ ко всем объектам этого раздела, которые используются при решении конкретной учебной задачи, в том числе и к регистрам.

Объекты должны быть сгруппированы по своему виду: справочники, документы, прочие объекты. Содержание остальных разделов определяется самостоятельно. 
Примерный вид интерфейса показан ниже:*

![Рисунок_ОУ1_1](https://user-images.githubusercontent.com/44517817/235097115-95c20495-6d40-4531-9a93-d9e5cbec9098.png)

*Картинки для оформления можно взять из библиотеки картинок — [файл piclib.dt](https://github.com/netology-code/onec-mid-homeworks/blob/main/OCPS/piclib.dt).

Компания занимается комиссионной торговлей. При приёме товара с комитентом заключается договор. 

Поступление товаров отражается документом «Приходная накладная». В каждой накладной указывается договор комиссии (договор — реквизит шапки), по которому поступил товар, и суммы по каждому товару.

Продажа отражается документом «Расходная накладная». В шапке документа должен быть указан сотрудник компании, осуществляющий продажу. 

Дополнительно для каждого товара в документе указывается договор комиссии, по которому этот товар к нам поступил. В случае если товара по этому договору нет, документ проводиться не должен. 

Кроме того, должен происходить контроль суммы, по которой продаётся товар. Сумма продажи не должна быть **ниже** указанной при поступлении товара по этому договору. В том случае, если одинаковый товар поступал по одному договору с указанием разных сумм, то при продаже **контролируемая сумма** рассчитывается как средняя по товару и договору.

Выплата комитенту происходит документом «Расход денег», в котором пользователем должно быть указано:
- по какому договору;
- какой товар;
- в каком количестве;
- на какую сумму был продан, но ещё не оплачен;
- сумма выплаты комитенту.

Предоплаты не предусмотрены. При проведении документа необходимо проверять, что мы не пытаемся рассчитаться с комитентом за большее количество товаров, **чем мы продали и чем мы уже отчитались перед ним**. Документ делается на одного комитента, но включает информацию по нескольким договорам.

Комиссионное вознаграждение рассчитывается исходя из условий договора, как процент от суммы продажи. Процент устанавливается в каждом договоре. Со временем значение процента может быть изменено, но историю его изменения в информационной базе хранить не надо.

Необходимо создать отчёты о продажах за период, о распределении выручки и о наличии товаров.

![image](https://github.com/netology-code/onec-mid-homeworks/assets/44517817/c5b004ba-e80d-424d-98cb-3ebf5e65af59)

Обязательно в пользовательском режиме заведите тестовый пример, приведённый в [файле «16.4. Исходные данные_ОУ3 к домашнему заданию.xlsx»](https://docs.google.com/spreadsheets/d/1sfbWzn1O4G2A3Jx6psvTa_7Va5kZHyDv/edit?usp=sharing&ouid=108088713556619645145&rtpof=true&sd=true).

------

### Самостоятельное задание 

Это задание предполагает самопроверку. Это означает, что вы сможете самостоятельно проверить его на наличие ошибок, которые приведены в [документе на сайте 1С, стр.#3, автозагрузка документа](https://static.1c.ru/rus/partners/training/files/ATT83PL.rtf?356jhteyner67j340).

Рекомендуем вам определить, сколько времени у вас занимает решение. Это поможет на экзамене правильно рассчитать свои временные ресурсы.

В личном кабинете вы отправляете ссылку на решение. Эксперт выборочно просматривает работы. А на следующем вебинаре разбирает частые ошибки, которые встречаются в работах слушателей.


Любые вопросы по решению задач задавайте в чате учебной группы.

*Примерное время выполнения: 45–180 минут.*
