---
layout: page
permalink: /privetstvie-v-sootvetstvii-s-vremenem-sutok/
---
# Приветствие в соответствии с временем суток

Для работы со временем будем использовать модуль [datetime](https://docs.python.org/3/library/datetime.html) и конкретно класс [datetime](https://docs.python.org/3/library/datetime.html#datetime.datetime). 
Так как класс в отдельном модуле, его необходимо предварительно импортировать, иначе получим ошибку:

```text.python.traceback
Traceback (most recent call last):
  File "<pyshell#0>", line 1, in <module>
    datetime.now()
NameError: name 'datetime' is not defined
```

Импорт производится простой командой: `from datetime import datetime`

Теперь осталось найти подходящую функцию в классе datetime, чтобы изменить написанную раннее `hello_func()`. 
Могу посоветовать вынести определение времени и приветствия во вспомогательную функцию(например, `choose_hello_phrase`), 
чтобы каждая функция имела одно назначение.

Решение не должно занять много времени, но показать несколько важных вещей:

1. Использовать документацию. В документации есть и особенности использования и изменения, внесённые в разных версиях.
2. Привыкать разделять функции, а потом и классы так, чтобы у каждого класса/функции была одна небольшая задача — это упрощает чтение и изменение кода

Вероятно, у вас уже возник вопрос, а как проверить, что функция работает — не ждать же каждое время суток. В следующий раз я затрону вопрос написания простых тестов.