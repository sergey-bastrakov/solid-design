﻿Как вы понимаете "Слабая связность (low coupling) и сильное зацепление (high cohesion)"?

	- Между модулями связи должны быть как можно слабже, а внутри модуля разные части должны быть сильно зацеплены друг за друга

Вот есть у меня большое приложение! И оно между собой связано! Это сильное зацепление. Все ли хорошо?

	- Нет. Раз приложение большое, то правильно разбить его на меньшие модули. Удачное разбиение, когда модули не будут зависеть друг от друга, т.е. иметь слабую связность. А вот если в них не будет сильного зацепления, значит их еще можно разбить.

Чем хороши маленькие модули?

	- Маленькие модули удобны, ведь их легко понять, протестировать и собрать что-то новое

Насколько надо мельчить?

	- Слишком сильное не стоит - станет неудобно!

Чем хороша слоистая архитектура?

	- В классической трехслойной архитектуре (представление, бизнес-логика, хранение данных) можно поменять архитектуру хранения или представления независимо от других слоев

Определите OCP? Что это означает на практике? Чем это хорошо?

	- Модуль открыт для расширения, но закрыт для модификации
	- Если мы хотим добавить новую функциональность, то в идеале мы не правим существующий код.
	- Минимальна вероятность ошибки

Приведите пример расширяемых систем?

	- ОС с помощью Applications
	- VisualStudio с помощью плагинов
	- JsonSerializer - переопределение серилизаций

Определите DIP?

	- Конкретика должна зависеть от абстракций, а не наоборот

Приведите примеры абстракции?

	- Абстракции - это интерфейсы, классы с виртуальными методами, делегаты

В чем практическая ценность DIP?

	- Абстракции можно подменять в тестах
	- Повышается переиспользуемость, ведь зависимости можно подменять