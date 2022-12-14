***Fragment*** - це частина інтерфейсу користувача. Перевага використання фрагментів полягає у тому, що одна [[Activity]] може містити кілька фрагментів.

Загалом, фрагментти можна розглядати як деякий модульний компонент з власним життєвим циклом.

**Фрагменти не можуть існувати самі по собі. Для робити їх необхідний хост - [[Activity]]. Життєвий цикл [[Activity]] безпосередньо впливає на життєвий цикл фрагменту.***

Управління фрагментами здійснюється за допомогою транзакцій. [[Транзакції]] дозволяють не тільки видаляти/додавати фрагменти, а й задавати анімаційні переходи, а також реалізувати стекову навігацію, аналогічну стековій навігації [[Activity]]. 