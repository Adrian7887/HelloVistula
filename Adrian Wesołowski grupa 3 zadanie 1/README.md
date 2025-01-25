Aplikacja umożliwia użytkownikowi wprowadzenie swojego imienia w parametrze URL, a następnie wyświetla spersonalizowane powitanie.

Frontend:
Aplikacja wykorzystuje Thymeleaf do dynamicznego renderowania strony HTML.
Strona HTML korzysta z atrybutu th:src, aby dynamicznie załadować obrazek z folderu static/images.
Backend:
Backend oparty na Spring Boot, obsługuje logikę aplikacji i zarządza żądaniami HTTP.
Główna funkcjonalność znajduje się w kontrolerze HelloController.
Działanie:
Parametr imienia w URL:

Użytkownik wprowadza swoje imię jako parametr name w URL, np.:
http://localhost:8080/greeting?name=Adrian.
Aplikacja przetwarza imię i wyświetla spersonalizowane powitanie, np.:
Cześć, Adrian!
Domyślna wartość:

Jeśli parametr name nie zostanie podany w URL, aplikacja przyjmuje domyślną wartość World i wyświetla:
Cześć, World!
Wyświetlanie obrazu:

Na stronie powitania wyświetlany jest obrazek, który jest przechowywany w folderze static/images.
Dynamiczne ładowanie obrazka odbywa się za pomocą atrybutu th:src w szablonie Thymeleaf.
