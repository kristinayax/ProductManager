### Описание задания:
Вам необходимо реализовать менеджер товаров, который умеет:

* добавлять товары в репозиторий,
* искать товары.

Что нужно сделать:

1. Разработайте базовый класс Product, содержащий ID, название, стоимость.   
2. Разработайте два унаследованных от Product класса: Book с текстовыми полями «название» и «автор» и Smartphone с текстовыми полями «название» и «производитель»; общие поля вынесите в родителя.    
3. Разработайте репозиторий, позволяющий сохранять Product, получать все сохранённые Product и удалять по ID. Для этого репозиторий будет хранить у себя поле с типом Product[] (массив товаров).   
4. Разработайте менеджера, который умеет добавлять Product в репозиторий и осуществлять поиск по ним. Для этого вам нужно создать класс, конструктор которого будет принимать параметром репозиторий, а также с методом publiс void add(Product product) и методом поиска.   

Менеджер при переборе всех продуктов, хранящихся в репозитории, должен для каждого продукта вызывать определённый в классе менеджера же метод matches, который проверяет, соответствует ли продукт поисковому запросу.

При проверке на соответствие запросу товара мы проверяем вхождение запроса в текст названия товара.

Напишите тесты на менеджер и репозиторий, добившись 100% покрытия по бранчам методов с логикой.
