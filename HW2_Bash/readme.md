## Задание 2 ##  
**1. Создать папку dir_1.**  
**2. Зайти в папку dir_1.**  
**3. Cоздать папку inner_dir_1.**  
**4. Посмотреть где ты находишься.**  
**5. Находясь в папку dir_1 создать пустой текстовый файл tf_1.txt.**  
**6. Находясь в папке dir_1 через команду cat создать текстовый файл tf_2.txt со следующими строками:  
the first 1, the second 2, the third 3.**  
**7. Зайти в папку inner_dir_1.**  
**8. Через cat сделать текстовый файл tf_3.txt  c любыми строками.**  
**9. Через cat добавить в текстовый файл tf_3.txt строку “the second 2."**  
**10. Через cat добавить в текстовый файл tf_3.txt строку “the sec 2”.**  
**11. Через cat добавить в текстовый файл tf_2.txt строку “the sec 3”.**  
**12. Через cat добавить в текстовый файл tf_3.txt строку “the SeCoNd 2.”**  
**13. Через cat добавить в текстовый файл tf_2.txt строку “the seConD 2”.**  
**14. Сделать текстовый файл tf_4.txt в котором будет 15 строк.**  
**15. Сделать текстовый файл tF_5.txt в котором будет 13 строк.**  
**16. Вывести список всех файлов в папке.**  
**17. Выйти из папки inner_dir_1.**  
**18. Вывести содержимое файла tf_3.txt в терминал.**  
**19. Найти путь к файлу tf_4.txt.**  
**20. Отчистить файл tf_4.txt от содержимого без удаления самого файла.**  
**21. Найти путь к файлам у которых есть  “tf” в названии.**  
**22. Найти путь к файлам у которых есть  “tf” в названии и буквы в любом регистре.**  
**23. Найти строки в файлах где есть комбинация букв “sec” в текущей папке.**  
**24. Найти строки в файлах где есть комбинация букв “sec” в любом регистре в текущей папке.**  
**25. Найти строки в файлах где есть только комбинация букв “sec” в текущей папке.**  
**26. Найти строки в файлах где есть только комбинация букв “sec” в любом регистре в текущей папке.**  
**27. Найти строки в файлах где есть комбинация букв “second” в текущей папке.**  
**28. Найти строки в файлах где есть комбинация букв “second” в любом регистре в текущей папке.**  
**29. Найти строки в файлах где есть комбинация букв “second” во всех папках ниже уровнем.**  
**30. Найти только путь и название файла в строках которых есть комбинация букв “second” в текущей папке.**  
**31. Найти все строки во всех файлах где нет комбинации “second”.**  
**32. Найти только название и путь к файлам где нет комбинации “second”.**  
**33. Вывести в терминал 4 последних строк любого текстового файла.**  
**34. Вывести в терминал 4 первые строки любого текстового файла.**  
**35. Команда в одну строку. Создать папку и создать текстовый файл с содержиммым.**  
**36. Команда в одну строку. Переместить в любую одну папку текстовые файлы у которых в содержимом есть слово “sec”.**  
**37. Команда в одну строку. Скопировать в любую одну папку текстовые файлы у которых в содержимом есть слово “sec”.**  
**38. Команда в одну строку. Найти все строки c “sec” во всех текстовых файлах, скопировать и вставить эти строки в один новый созданный текстовый файл.**  
**39. Команда в одну строку. Удалить текстовые файлы у которых в содержимом есть слово “sec”.**  
**40. Просто вывести в терминал строку “Good job!!”.**  
## Решение ##
**1.Создать папку dir_1**  
```bash
mkdir dir_1
```
**2.Зайти в папку dir_1**  
```bash
cd dir_1
```  
**3. создать папку inner_dir_1**  
```bash
mkdir inner_dir_1
```  
**4. Посмотреть где ты находишься**  
```bash
pwd
```  
**5. Находясь в папку dir_1 создать пустой текстовый файл tf_1.txt**  
```bash 
touch tf_1.txt
```  
**6. Находясь в папке dir_1 через команду cat создать текстовый файл tf_2.txt со следующими строками:**  
- the first 1
- the second 2
- the third 3

```Bash
cat > tf_2.txt
```  
  Ввести строки  
  Нажать ctrl+c  

**7. Зайти в папку inner_dir_1**  
```bash
cd inner_dir_1
```  
 **8. Через cat сделать текстовый файл tf_3.txt  c любыми строками**  
 **9. Через cat добавить в текстовый файл tf_3.txt строку “the second 2"**  
 **10. Через cat добавить в текстовый файл tf_3.txt строку “the sec 2”**  
 **12. Через cat добавить в текстовый файл tf_3.txt строку “the SeCoNd 2”**  
```bash 
cat > tf_3.txt
```  
  Ввести строки из п.8-10,12  
  Нажать ctrl+c

**11. Через cat добавить в текстовый файл tf_2.txt строку “the sec 3”**  
**13. Через cat добавить в текстовый файл tf_2.txt строку “the seConD 2”**  
```bash
cat >> ../tf_2.txt
```  
  Ввести строки из п.11,13  
  Нажать ctrl+c  

**14. Сделать текстовый файл tf_4.txt в котором будет 15 строк.**  
```bash
nano tf_4.txt
```  
**15. Сделать текстовый файл tF_5.txt в котором будет 13 строк.**  
```bash 
nano tF_5.txt 
```
**16. Вывести список всех файлов в папке.**  
```bash
ls -la
```
```bash
ls -lR | grep ^-
```
**17. Выйти из папки inner_dir_1**  
```bash
cd ..
```
**18. Вывести содержимое файла tf_3.txt в терминал.**  
```bash
cat inner_dir_1/tf_3.txt
```  
**19. Найти путь к файлу tf_4.txt**  
```bash
find -name tf_4.txt
```  
**20. Отчистить файл tf_4.txt от содержимого без удаления самого файла.**  
```bash 
echo > tf_4.txt
```
**21. Найти путь к файлам у которых есть  “tf” в названии.**  
```bash
find -name "*tf*"
```
**22. Найти путь к файлам у которых есть  “tf” в названии и буквы в любом регистре.**  
```bash
find -iname "*tf*"
```
**23. Найти строки в файлах где есть комбинация букв “sec” в текущей папке**  
```bash
grep sec *
```
**24. Найти строки в файлах где есть комбинация букв “sec” в любом регистре в текущей папке**  
```bash
grep -i sec *
```
**25. Найти строки в файлах где есть только комбинация букв “sec” в текущей папке**  
```bash
grep -w sec *
```
**26. Найти строки в файлах где есть только комбинация букв “sec” в любом регистре в текущей папке**  
```bash
grep -iw sec *
```
**27. Найти строки в файлах где есть комбинация букв “second” в текущей папке**  
```bash
grep second *
```
**28. Найти строки в файлах где есть комбинация букв “second” в любом регистре в текущей папке**  
```bash
grep -i second *
```
**29. Найти строки в файлах где есть комбинация букв “second” во всех папках ниже уровнем**  
```bash
grep -d recurse second */.
```
или  
```bash
grep -r second */.
```
**30. Найти только путь и название файла в строках которых есть комбинация букв “second” в текущей папке**  
```bash
grep -l second *
```
**31. Найти все строки во всех файлах где нет комбинации “second”**  
```bash
grep -vr second *
```
**32. Найти только название и путь к файлам где нет комбинации “second”**  
```bash
grep -rL second *
```
**33. Вывести в терминал 4 последних строк любого текстового файла**  
```bash
teil -n4 inner_dir_1/tf_5.txt
```
**34. Вывести в терминал 4 первые строки любого текстового файла**  
```bash
head -4 inner_dir_1/tf_5.txt
```
**35. Команда в одну строку. Создать папку и создать текстовый файл с содержиммым**  
```bash
cat > tf_6.txt|mkdir ../dir_2 
```
Вводим содержимое  
Ctrl+c  
**36. Команда в одну строку. Переместить в любую одну папку текстовые файлы у которых в содержимом есть слово “sec”**  
```bash
 grep -wrl sec *| xargs mv -t ../dir_2
```
**37. Команда в одну строку. Скопировать в любую одну папку текстовые файлы у которых в содержимом есть слово “sec”**  
```bash
 grep -wrl sec ..| xargs cp -t inner_dir_1/
```
**38. Команда в одну строку. Найти все строки c “sec” во всех текстовых файлах, скопировать и вставить эти строки в один новый созданный текстовый файл**  
```bash
grep -rh --line-buffered sec .. > new_tf.txt
```
**39. Команда в одну строку. Удалить текстовые файлы у которых в содержимом есть слово “sec”**  
```bash
grep -wrl sec ..| xargs rm
```
**40. Просто вывести в терминал строку “Good job!!”**  
```bash
echo Good job!!
```
