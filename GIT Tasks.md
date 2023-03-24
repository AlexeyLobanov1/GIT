1. На локальному репозиторії створити гілки для:
- Postman      (git checkout -b Postman)
- Jmeter       (git checkout -b Jmeter)
- CheckLists   (git checkout -b CheckLists)
- Bug Reports  (git checkout -b BugReports)
- SQL          (git checkout -b SQL)
- Charles      (git checkout -b Charles)
- Mobile testing  (git checkout -b Mobiletesting )
2. Запушити всі гілки на віддалений репозиторій   (git push –all origin)

3. У гілці Bug Reports створити текстовий документ txt зі структурою Баг Репорту.
(git checkout BugReports , touch BugReport.txt)

4. Запушити структуру Баг Репорту на зовнішній репозиторій.
(git add .    git commit -m ‘BugReport: structure’   git push -u origin BugReports)

5. Замержити гілку Bug Reports з гілкою main.
```bash
git checkout main
git merge BugReports
git push
```

6. У гілці CheckLists створити структуру чек-листа.
( git checkout CheckLists,    touch CheckList.txt)

7. Запушити структуру чек-листа на зовнішній репозиторій.
(git add .    git commit -m ' Checklist: structure’   git push -u origin CheckLists)

8. На зовнішньому репозиторії зробити Pull Request гілки CheckLists в гілку Main.
(git checkout main   git merge CheckLists    git push )

9. Синхронізувати зовнішню та локальну гілки Main.
(git checkout main   git pull   git push origin main )

Завдання JSON Частина 2
1.Створити зовнішній репозиторій з назвою JSON.
- зашёл в github создал Json

2.Склонувати репозиторій JSON на локальний комп'ютер.
- mkdir git.json   cd git.json  git clone URL

3.В локальному репозиторії JSON створити файл "new.json".
- touch new.json   

4.Додати файл до індексу Git (щоб гіт відслідковував цей файл).
- git add new.json
            
5.Закомітити файл. 
- git commit -m 'add new.json' 

6.Відправити файл у зовнішній репозиторій GitHub.
- git push origin main

7.Відредактувати вміст файлу “new.json” - написати інформацію про себе (ФІО, вік, кількість домашніх тварин, майбутня бажана зарплата). Все написати у форматі JSON
{
    "name": "Lobanov Alexey",
    "age": 23,
    "pets": 1,
    "salary": "10000$"
}

8.Відправити зміни на зовнішній репозиторій.
- git push origin main 

9.Створіть файл preferences.json
- touch preferences.json

10.У файл preferences.json додайте інформацію про своїх перевагах (Любимий фільм, улюблений серіал, улюблена еда, улюблене час року, сторони хотіли б відвідати) у форматі JSON  
 {
 "favorite_movie": "Matrix",
    "favorite_tv_show": "1,000 Ways to Die",
    "favorite_food": "Pizza",
    "favorite time of the year": "Autumn",
    "Countries I'd like to visit": "France"
  }

11.Створіть файл sklls.json, додайте інформацію про навички, які будуть вивчатися на курсі у форматі JSON
-  touch skIls.json 
{
  "Testing": ["Theory", "test design techniques"],
  "Documentation": ["Test cases", "checklists", "bug reports"],
  "Tools": ["Chrome DevTools", "Postman", "Swagger","GraphQL"]
}

12.Відправити відразу 2 файли на зовнішній репозиторій.
- git add .     git commit -m 'Add preferences.json and skills.json'   git push origin main

13.На веб-інтерфейсі створіть файл bug_report.json.
- Зашел в github зашел в репозиторий,нажал Create new file назвал bug_report.json

14.Зробити зафіксовані зміни (зберегти) зміни на веб-інтерфейсі.
- Commit new file

15.У веб-інтерфейсі модифікуйте файл bug_report.json, додайте пакет звіту у форматі JSON.
{
 "Title": "Registration error",
  "Preconditions": ["Go to https//:kokoine", "credantials: login alex password: 1234"],
  "Steps_to_reproduce": "enter data from the credantials and press register",
  "Expected_result": "Registration is successful",
  "Actual_result": "Error 403"
}

16.Сделать Зафіксувати зміни (зберегти) зміни на веб-інтерфейсі.
- Commit new file

17.Синхронізувати зовнішній і локальний репозиторій JSON.
- cd git.json      git pull



