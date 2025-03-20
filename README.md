# lab2.3_obd
# ЛАБОРАТОРНА РОБОТА №3
# Створення та аналіз запитів у MS SQL
**Короткий опис**

У цій лабораторній роботі показано виконання багатотабличних запитів, які включають в себе використання різних типів **JOIN** для об'єднання таблиць, що дозволяє отримувати дані з кількох джерел. 
Використання **каскадних дій** забезпечує цілісність даних при виконанні операцій, таких як оновлення або видалення. Опанування **сортуванням** результатів 
запитів дозволяє організувати дані за певним критерієм. Застосування **булевих** та **реляційних операторів** допомагає фільтрувати дані на основі умов. Крім того, 
важливо **аналізувати продуктивність SQL-запитів** для оптимізації їх виконання.

**Завдання 3**
Розгортання MS SQL на Docker:
![image](https://github.com/user-attachments/assets/40cb6454-31ff-42f7-b9ca-2c715fd7cafa)
Вхід до контейнеру та створення бази:
![image](https://github.com/user-attachments/assets/3bc93d82-612e-4710-93d6-95b007653975)
Копіювання скриптів до контейнеру:
![image](https://github.com/user-attachments/assets/57fa097a-ac30-431c-8654-c5405d59cb64)
![image](https://github.com/user-attachments/assets/057174bd-e880-4463-8de3-67ed2f96a584)
Запуск скриптів:
![image](https://github.com/user-attachments/assets/c02152d6-035e-4a95-8fcd-265fbae25091)

**Завдання 4**
--Запит про тварин, їх вакцинацію та доглядачів
![image](https://github.com/user-attachments/assets/f3beea55-6a13-4c29-9629-6c39526744ee)
--Запит про вагу тварин та корм, який їм дають
![image](https://github.com/user-attachments/assets/862f4ab1-2b3d-483b-8ef6-076d03bc825c)

**Завдання 5**
--Запит для оновлення даних у таблиці Animal і каскадне оновлення у таблиці Family
UPDATE Animal
SET Gender = 'female'
WHERE Nickname = 'Bella';

--Запит для видалення запису з таблиці Animal і каскадне видалення в таблицях Vaccination та Caretaker
DELETE FROM Animal
WHERE Nickname = 'Max';

**Завдання 6**
--Сортування тварин за віком (за зростанням)
![image](https://github.com/user-attachments/assets/667c2113-72e0-402a-b803-73b877ae25b3)
--Сортування тварин за алфавітом (Nickname)
![image](https://github.com/user-attachments/assets/3ca94b4a-4bca-4e73-8281-2571b06c96d5)

**Завдання 7**
--Використання булевого оператора AND та реляційних операторів для вибірки тварин за віком і кількістю поросят
![image](https://github.com/user-attachments/assets/5e5a2e3c-d097-4a4d-a907-a5a3217d1be6)
--Використання булевого оператора OR та реляційних операторів для вибірки тварин з певними умовами
![image](https://github.com/user-attachments/assets/994dca0c-ee94-4915-9b1f-290e1cfeb524)

**Завдання 8**
-- LEFT JOIN для вибірки всіх тварин з інформацією про вакцинацію
![image](https://github.com/user-attachments/assets/8867a0d4-056b-48fc-a040-12cf07951cef)
--FULL JOIN для вибірки всіх тварин та доглядачів, включаючи ті, для яких немає відповідності
![image](https://github.com/user-attachments/assets/7dce67bc-3706-4b5c-a4f4-9fe8ac4df976)

**Завдання 9**
--Групування тварин за їхнім призначенням та фільтрація за кількістю поросят
![image](https://github.com/user-attachments/assets/8d39fe6d-f9e6-4721-95d3-a03d8208eb39)
--Групування тварин за статтю та фільтрація за середньою кількістю поросят
![image](https://github.com/user-attachments/assets/069f2f27-4f6e-4170-a416-f567da9e4827)
--Групування тварин за їхнім статтю і призначенням з фільтрацією за кількістю вакцинацій
![image](https://github.com/user-attachments/assets/a4d380bd-4850-40bb-9467-20d43661bfdb)
--Групування доглядачів за тваринами і фільтрація за середнім віком тварин
![image](https://github.com/user-attachments/assets/dc7bd9b4-6564-47ce-a29e-163fc175917e)
--Групування кормів за місяцем та фільтрація за середньою кількістю корму
![image](https://github.com/user-attachments/assets/3fcf4fdd-de39-4a94-b2a5-67fe7d93616e)
**Завдання 11**
![image](https://github.com/user-attachments/assets/9405ba18-d38c-40b4-bb8f-9d01ee2bcb32)
