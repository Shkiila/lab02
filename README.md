# TIMP_Lab02

# Part I

## Задание №1
```
https://github.com/JeySie00/TIMP_Lab02
```
## Задание №2
```
git clone https://github.com/JeySie00/TIMP_Lab02
git add README.md
git commit -m "Create README.md"
git push
```
## Задание №3
```
cat > "Hello_world.cpp" << EOF
#include <iostream>

using namespace std;
int main(int argc, char** argv){
    cout << "Hello world" << endl;
}
EOF
```
## Задание №4
```
git add hello_world.cpp
```
## Задание №5
```
git commit -m "Add hello_world.cpp"
```
## Задание №6
Отредактировано в Visual Studio Code
```
#include <iostream>
#include <string>

using namespace std;
int main(int argc, char** argv){
    cout << "Hello world" << endl;
    string name;
    cin >> name;
    cout << "Hello world from " << name << endl;

```
## Задание №7
```
git commit -m "Changed hello_world.cpp"
```
## Задание №8
```
git push
```
## Задание №9
```
История коммитов доступна в удалёном репозитории
```

# Part II
## Задание №1
```
git checkout -b patch1
```
## Задание №2
Отредактировано в Visual Studio Code
```
#include <iostream>
#include <string>
 
int main(int argc, char** argv){
    string name;
    std::cin >> name;
    std::cout << "Hello world from " << name << std::endl;
}
```
## Задание №3
```
git commit -m "Fixed"
git push --set-upstream origin patch1
```
## Задание №4
```
Ветка patch1 доступна в удалённом репозитории
```
## Задание №5
```
Создадим pull-request patch1 -> main
```
## Задание №6
Отредактировано в Visual Studio Code
```
#include <iostream>
#include <string>
 
int main(int argc, char** argv){
    string name; // User name
    std::cin >> name; // Input user name
    std::cout << "Hello world from " << name << std::endl;
} 
```
## Задание №7
```
git commit -m "Add comments"
git push --set-upstream origin patch1
```
## Задание №8
```
Новые изменения есть в созданном на шаге 5 pull-request
```
## Задание №9
```
 В удалённом репозитории выполняем слияние PR patch1 -> master и удаляем ветку patch1 в удаленном репозитории.
```
## Задание №10
```
git pull
```
## Задание №11
```
git log
```
## Задание №12
```
git branch -d patch1
```
# Part III
## Задание №1
```
git checkout -b patch2
```
## Задание №2
```
clang-format -i -style=Mozilla "Hello_world.cpp"
```
## Задание №3
```
git commit -m "Changed code style"
git push --set-upstream patch2
```
## Задание №4
```
В ветке master в удаленном репозитории изменяем комментарии

#include <iostream>
#include <string>
 
int main(int argc, char** argv){
    string name; // Имя пользователя
    std::cin >> name; // Ввод имени пользователя
    std::cout << "Hello world from " << name << std::endl; //Печать "Hello world from (имя польвователя)"
}  
```
## Задание №5
```
Убеждаемся, что в pull-request появились конфликтны.
```
## Задание №6
```
git checkout main
git pull
git rebase
git commit -m "Update Hello world.cpp"
```
## Задание №7
```
git push --set-upstream patch2
```
## Задание №8
```
Убеждаемся, что в pull-request пропали конфликтны.
```
## Задание №9
```
Выполняем merge pull-request patch2 -> main
```
