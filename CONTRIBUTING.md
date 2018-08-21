# Руководство по созданию нового pull request

Pull request позволяет команде просмотреть код и дать отзыв об изменениях, прежде чем смерджить его. Можно указать ветку (branch), в которую передать pull request. Ответственные за проверку кода (reviewers) могут принять либо отклонить изменения.
# Из Visual Studio

1. Подключите проект через Team Explorer

![](https://github.com/Erlanici/Draw/blob/master/img/1%20(2).png?raw=true)

![](https://github.com/Erlanici/Draw/blob/master/img/2018-08-21_14-08-46%20(2).png?raw=true)

Панель Team Explorer должна выглядеть примерно как на картинке ниже. Плагин GitFlow ставится отдельно (https://marketplace.visualstudio.com/items?itemName=vs-publisher-57624.GitFlowforVisualStudio2017).

![](https://github.com/Erlanici/Draw/blob/master/img/2018-08-21_14-09-36.png?raw=true)

2.  Получаем последнюю рабочую версию проекта и создаем новую features в GitFlow. Название фичи начните с номера задачи, например, t123NewFeatures. Не забудьте убедиться, что в том, что созданная вами фича стало активной веткой.

![](https://github.com/Erlanici/Draw/blob/master/img/2018-08-21_14-11-24%20(2).png?raw=true)

4. Вносим изменения в код.
5. Закоммитьте изменения. В комментарии укажите номер задачи через '#'.

![](https://github.com/Erlanici/Draw/blob/master/img/2018-08-21_14-24-07%20(2).png?raw=true)

7. Если вы еще не отправляли ветвь, как это указано на картинке ниже, то сделайте это. После это станет доступным пункт меню "Create Pull Request".

![](https://github.com/Erlanici/Draw/blob/master/img/2018-08-21_14-24-40%20(2).png?raw=true)

9. Создаем Pull request, согласно схеме что указана ниже.

![](https://github.com/Erlanici/Draw/blob/master/img/2%20(2).png?raw=true)

10. При успешном выполнении откроется окно браузера на сайте VSTS. Нужно будет убедиться, что та ветка, куда будут влиты изменения, это ветка develop. Задайте заголовок, укажите номер задачи через '#' (#num такой способ записи связывает нас с задачей). Выберете лиц, ответственных за внесение изменений (Reviewer), если вы забыли их указать, то это можно сделать после. Если в пункте "Work Items" задача автоматически не подтянулась, то можно её найти по номеру и выбрать. После всех приготовлений жмем кнопку Create.

![](https://github.com/Erlanici/Draw/blob/master/img/2018-08-21_15-22-17%20(2)-min-min-min.png?raw=true)

11. Если изменения были отклонены, то читаем комментарии и исправляем код, возвращаемся к пункту 4. 
12. Когда изменения будут приняты, переключаемся на ветку develop, получаем последние изменения.

![](https://github.com/Erlanici/Draw/blob/master/img/2018-08-21_15-53-46.png?raw=true)

13. Закрываем фичу. Переключаемся в GitFlow, если вы находитесь в ветке develop, то выбираем Other => Finish Feature. Если вы переключились на ветку фичи, то сразу будет доступно удаление.

![](https://github.com/Erlanici/Draw/blob/master/img/2018-08-21_15-55-25.png?raw=true)
![](https://github.com/Erlanici/Draw/blob/master/img/2018-08-21_15-57-19.png?raw=true)

**Note: *для выполнения pull request ставить gitflow не обязательно, но это облегчает работу.***
