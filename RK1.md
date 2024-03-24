**1. Название проекта:**  

*30-seconds-of-cpp*

**2. Краткое описание проекта(одной фразой):**  

*30 Seconds of C++ (STL in C++). Read More about 30C++ here*

**3. Количество файлов:**  
```
tree -a | tail -1
```
*39 directories, 413 files*

**4. Объем всех файлов:**  
```
du -sh  .
```
*4,2M	.*

**5. Объем исходного кода: cpp, c, h, hpp, cxx, py, pl, php, java, cs, rb, rs, hs:**  

```
find . -type f -name "*.cpp" -ls | awk '{sum+=$7} END {print sum}'
```
*88522*  

```
find . -type f -name "*.py" -ls | awk '{sum+=$7} END {print sum}'
```
*7458*  

**6. Найти, если есть файл .clang-format: ./.clang-format:**
```
find . -name ".clang-format"
```
*Нет файла*  

**7. Каталог src:**
```
find . -name "src"
```
*Нет файла*  

**8. Выписать количество файлов, содержащих слово socket не зависимо от написания:**
```
grep -irl "socet" . | wc -l
```
*0*  

**9. Выписать количество файлов, содержащих слово select не зависимо от написания:**
```
grep -irl "socet" . | wc -l
```
*0*  

**10. Выписать количество раз, сколько встречается слово Microsoft, Google или Intel не зависимо от написания:**
```
grep -ir -e "Google" -e "Microsoft" -e "Intel" | wc -l
```
*2*

**11. Найти расположение файла LICENSE относительно начала репозитория:**
```
find . -name "LICENSE" -type f
```
*./LICENSE*  

**12.Вывести строку для файла LICENSE(если она есть), в которой есть аббревиатура BSD, GNU, MIT, APSL, Apache, GPL, AGPL, LGPL:**
```
cat LICENSE | grep -i -e "BSD" -e " GNU " -e " MIT " -e " APSL " -e " Apache " -e " GPL " -e " AGPL " -e " LGPL  "
```
*Нет таких аббревиатур*























