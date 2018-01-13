# How to work with GIT

Ми cтворили файл ===> git add назва файлу
Ми внесли змінни в файл ===> git commit -am "опис коміту"
Ми хочемо відправити зміни на сервер ===> git push origin назва-гілки

Ми хочемо працювати в новій гілці ===> git checkout -b назва-нової-гілки
Ми хочемо повернутись до старої гілки або перейти на іншу ===> git checkout назва-гілки

Ми хочемо оновити нашу гілку до останнього стану:
    1) git checkout master (Або основну)
    2) git pull origin master (Або основну) ===> оновлюємо master до останньої версії
    3) git checkout назва-гілки 
    4) git merge master (Або основну) ===> Ми зливаємо (всі змінни що є в master) гілку master в нашу гілку
    5) Можуть виникнути конфлікти
        1) в едіторі залишаємо ті частини коду які нас влаштовують
        2) git add імя-файлу-з-конфліктами
        3) git commit -am "Merge Master"
    6) git push origin назва-гілки

