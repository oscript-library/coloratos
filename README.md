# Цветной вывод
## Библиотека oscript для цветного вывода в консоль  

----------------------------------------------------

Вывод формируется по шаблону `(Текст|#color=Цвет)`, где  
- `Текст` - произвольный текст  
- `Цвет` - строковое значение перечисления `ЦветКонсоли.*`


Примеры использования:
```bsl
#Использовать ".."

ЦветнойВывод.Вывести("Процесс выполнения... ", "Серый");
ЦветнойВывод.ВывестиСтроку("Done", "Зеленый");
``` 
> Результат:  
![doc/capture1.png](doc/capture1.png)

```bsl
#Использовать ".."
ЦветнойВывод.ВывестиСтроку(
		"(Оу!|#color=White) Привет, (Красный!|#color=Красный) Кажется я выгляжу '(малиновым|#color=Малиновый)'.
		|Ты тоже видишь (желтый текст|#color=Желтый) ???", "Синий");
```
> Результат:  
![doc/capture2.png](doc/capture2.png)

-------------------------------------------------
Больше примеров см. в [test/test.os](test/test.os)