# grep

## Lesson Content

Команда grep, возможно наиболее важная команда, в отношении обработки текста, которую вы будете использовать. Она позволяет вам искать файлы по особенностям, которые совпадают с некоторым шаблоном. Что если бы вы хотели знать, существует ли файл в некоторой директории, или если бы вы хотели узнать, есть ли строка в файле? Конечно, вам не придется копаться в каждой строчке текста, вы будете использовать grep!

Давайте будем использовать наш файл sample.txt как пример:

<pre>$ grep fox sample.txt</pre>

Вы должны увидеть, что grep нашел fox в нашем sample.txt.

Вы также можете задавать шаблоны, которые не чувствительны к регистру с флагом -i:

<pre>$ grep -i somepattern somefile</pre>

Чтобы получить большую гибкость с grep вы можете сочетать его с другими командами с |.

<pre>$ env | grep -i User</pre>

Как вы можете видеть, grep довольно универсален. Вы даже можете использовать регулярные выражения в вашем шаблоне:

<pre>$ ls /somedir | grep '.txt$'</pre>

Должно вернуть все файлы, оканчивающиеся на .txt в директории somedir.

## Exercise

Возможно, вы слышали о egrep или fgrep, эти устаревшие вызовы grep заменены на grep -E и grep -F. Прочитайте man grep, чтобы узнать больше.

## Quiz Question

Какая команда используется для поиска по шаблону?

## Quiz Answer

grep