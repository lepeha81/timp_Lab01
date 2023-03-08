# timp_Lab01
# Homework
1. Скачайте библиотеку *boost* с помощью утилиты **wget**. Адрес для скачивания `https://sourceforge.net/projects/boost/files/boost/1.69.0/boost_1_69_0.tar.gz`.
2. Разархивируйте скаченный файл в директорию `~/boost_1_69_0`
3. Подсчитайте количество файлов в директории `~/boost_1_69_0` **не включая** вложенные директории.
4. Подсчитайте количество файлов в директории `~/boost_1_69_0` **включая** вложенные директории.
5. Подсчитайте количество заголовочных файлов, файлов с расширением `.cpp`, сколько остальных файлов (не заголовочных и не `.cpp`).
6. Найдите полный пусть до файла `any.hpp` внутри библиотеки *boost*.
7. Выведите в консоль все файлы, где упоминается последовательность `boost::asio`.
8. Скомпилирутйе *boost*. Можно воспользоваться [инструкцией](https://www.boost.org/doc/libs/1_61_0/more/getting_started/unix-variants.html#or-build-custom-binaries) или [ссылкой](https://codeyarns.com/2017/01/24/how-to-build-boost-on-linux/).
9. Перенесите все скомпилированные на предыдущем шаге статические библиотеки в директорию `~/boost-libs`.
10. Подсчитайте сколько занимает дискового пространства каждый файл в этой директории.
11. Найдите *топ10* самых "тяжёлых".
## Выполнение
1.
![image](https://github.com/lepeha81/timp_Lab01/blob/main/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA1.PNG)
wget ... - скачивание файла и сохранение в текущей директории\
2.
![image](https://github.com/lepeha81/timp_Lab01/blob/main/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA3.PNG)
tar -xf - распаковка файла\
tar -C - используется для указания папки\
3.
![image](https://github.com/lepeha81/timp_Lab01/blob/main/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA4.PNG)
find -type f - искать файлы\
Команда find передаёт список всех файлов в текущем каталоге с каждым именем файла в одной строке команде wc, которая подсчитывает количество строк и печатает результат\
4.
![image](https://github.com/lepeha81/timp_Lab01/blob/main/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA5.PNG) 
5.
![image](https://github.com/lepeha81/timp_Lab01/blob/main/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA6.PNG)
![image](https://github.com/lepeha81/timp_Lab01/blob/main/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA7.PNG)
![image](https://github.com/lepeha81/timp_Lab01/blob/main/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA8.PNG)
6.
![image](https://github.com/lepeha81/timp_Lab01/blob/main/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA9.PNG)
7.
![image](https://github.com/lepeha81/timp_Lab01/blob/main/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA19.PNG)
grep -r - Первый параметр представляет регулярное выражение для поиска, а второй представляет каталог, в котором необходимо искать. В данном случае имеется в виду текущий каталог\
8.
![image](https://github.com/lepeha81/timp_Lab01/blob/main/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA10.PNG)
![image](https://github.com/lepeha81/timp_Lab01/blob/main/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA11.PNG)
./script.sh - запуск скрипта\
--prefix=PREFIX - папка для установки программы\
9.
![image](https://github.com/lepeha81/timp_Lab01/blob/main/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA12.PNG)
![image](https://github.com/lepeha81/timp_Lab01/blob/main/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA13.PNG)
![image](https://github.com/lepeha81/timp_Lab01/blob/main/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA14.PNG)
mv - переместить файлы или директории\
10.
![image](https://github.com/lepeha81/timp_Lab01/blob/main/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA17.PNG)
du -a - вывод размера папок и файлов\
11.
![image](https://github.com/lepeha81/timp_Lab01/blob/main/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA18.PNG)
sort -n -r - сортировка строк по числовому значению в обратном порядке\
head -n - вывод 10 строк
