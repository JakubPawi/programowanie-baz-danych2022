# programowanie-baz-danych2022
O aplikacji

Aplikacja New Songs Relases (w skrócie NSR) informuje użytkownika o nowych utworach artysty. Należy wpisać nazwę artysty, by móc na bieżąco śledzić nowości danej osoby. Strona aplikacji posiada wyszukiwarkę, gdzie można wpisać nazwę wykonawcy. Za pomocą ogólnodostępnego (API ze Spotify) wyświetli się dany wykonawca z nowym utworem.

image

Uruchomienie

Aby uruchomić aplikację musimy przygotować plik .env i w miejsce CLIENT_ID i CLIENT_ID_SECRET wkleić otrzymane wartości od Spotify Web API. Następnie musimy wykonać w CMD następujące komendy:

composer install
npm install
php artisan key:generate
php migrate 
php artisan serve

Licencja

Spotify-Web-Api-PHP również na licencji MIT i Spotify Web Api użyte w celach edukacyjnych.

Autorzy

Hubert Łebkowski
Szymon Ludwiński
Jakub Pawiński

Specyfikacja wymagań
Definicja wymagania(scenariusz) 	Użytkownik wyszukuje blibliotekę piosenek i albumów, a wśród nich najnowsze wydanie
Aktorzy 	Użytkownik chcący wyszukać najnowszy utwór
Warunki początkowe 	Użytkownik wchodzący na stronę internetową
Przebieg realizacji scenariusza 	

    Użytkownik wchodzi na stronę internetową
    W odpowiednim polu wpisuje nazwę artysty, którego chce wyszukać i klika przycisk
    System wyświetla katalog piosenek i albumów, wskazując najnowszy(zmieniając tło na żółte)


Wymagania funkcjonalne

    użytkownik będzie mógł przeszukać katalog utwórów i albumów danego artysty
    strona internetowa udostępni katalog utwóró i albumów danego artysty


Wymagania niefunkcjonalne

    dostępność/niezawodność - strona powinna być dostępna cały czas
    wydajność - strona powinna w szybkim czasie zwracać katalog utworów i albumów
    użyteczność - po wyszukaniu od razu mamy informację, który utwór jest najnowszy

Architektura systemu

Stos technologiczny - architektura rozwojowa

    Visual Studio Code (IDE)
    Laravel
    Spotify Web API

Stos technologiczny - architektura uruchomieniowa

    PHP,CSS,JavaScript
    Laravel,jQuery
    BootStrap 4
    npm, artisan
    MySQL
    Git

Testy

    Test sprawdzający czy Token został dodany do bazy danych co ma kluczowe znaczenie dla działania całej aplikacji
