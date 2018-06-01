# Домашняя работа №9.
1. Первым заданием было удалить все строки. Я использовала регулярное выражение ^\s+. Я использовала графу "Find". Графу "Replace" я оставила пустой. 
![screenshot of 1](https://github.com/polinafanaseva/result.txt/blob/master/1.jpg)
2. Вторым заданием было найти всех князей и города, имя и название которых оканчивается на "слав". При этом в выдаче должны были быть такие слова как "Ярославля, Ростиславъ, Ростиславу, Переяславлъ" и т.п., но не должно было быть "славу, выславше" и т.п. Я использовала регулярное выражение [А-ЯѢ]+[а-яѣ]+(слав)[а-яѣ]+ . Всего было найдено 564 совпадения.
![screenshot of 2](https://github.com/polinafanaseva/result.txt/blob/master/2.jpg)
3. Третьим заданием было найти все упоминания Новгорода. Я использовала регулярное выражение (Нов)+.(город)[^W]. Всего было найдено 58 совпадений.
![screenshot of 3](https://github.com/polinafanaseva/result.txt/blob/master/3.jpg)
4. В бонусном задании необходимо было после каждого знака препинания поставить пробел (но выставлять их стоит только если того требуют правила русского языка). Я разделила задание на 3 регулярных выражения.

№1 Чтобы выполнить эти условия:
-надо добавить пробел после двоеточия
-надо добавить пробел после точки с запятой
-надо добавить пробел после запятой
я  использовала регулярное выражение ([!,.;:"]) с заменой на \1 
![screenshot of 4](https://github.com/polinafanaseva/result.txt/blob/master/4.jpg)

№2 Чтобы выполнить это условие: 
- перед квадратной скобкой должен быть пробел; 
я использовала регулярное выражение (\[) с заменой на  \1.
![screenshot of 5](https://github.com/polinafanaseva/result.txt/blob/master/5.jpg)

№3 Чтобы выполнить это условие:
- после точки должен быть пробел, если до нее буква или кавычка, а после нее нет другой точки 
- исключить наличие пробелов между точкми в многоточии
я использовала регулярное выражение \.  \.  \.   с заменой на ... 
![screenshot of 6](https://github.com/polinafanaseva/result.txt/blob/master/6.jpg)

И в конце, привела текст в нормальный вид, заменив 2,3,4,5-ые пробелы одним. 
