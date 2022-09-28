## https://learn.javascript.ru/first-steps

### (1) Chapter - https://learn.javascript.ru/while-for

### Description: 
Повторять цикл, пока ввод неверен.<br/>
Напишите цикл, который предлагает prompt ввести число, большее 100. Если посетитель ввёл другое число – попросить ввести ещё раз, и так далее.<br/>
Цикл должен спрашивать число пока либо посетитель не введёт число, большее 100, либо не нажмёт кнопку Отмена (ESC).Предполагается, что посетитель вводит только числа. Предусматривать обработку нечисловых строк в этой задаче необязательно.
 
### Solution: 
  ```javascript
  "use strict";
   let num;
  do {
  let num = prompt('Введите число больше 100?','');
    if (num > 100) {
      alert("correct!");
      break;
    } else if (num === null ){
      alert("close");
      break;
    } else if  (num === '' || num <= 100)  {
      alert("uncorrect!")
    }
  } while (true);
   ```
