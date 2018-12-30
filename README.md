<h1>Komunikator internetowy</h1>
<p>Jest to prosta aplikacja internetowa zbudowana w oparciu o technologie Spring 5 oraz Angular 7 i jednocześnie projekt
zaliczeniowy na przedmiot Programowanie aplikacji internetowych</p>
<p>Elementy aplikacji</p>
<ul>
<li><strong>Integracja z bazą danych H2</strong> - serwer komunikuje się z bazą danych w celu zapisywania i odczytywania danych dotyczących
użytkowników, grup i wiadomości. Cała komunikacja oparta jest na Spring JPA i Spring Data.</li>
<li><strong>Rejestracja nowych użytkowników</strong> - Aby móc korzystać z aplikacji, konieczne jest posiadanie konta. Specjalny formularz
pozwala na podanie danych takich jak nazwa użytkownika, hasło. Dane te są poddawane sprawdzeniu i zapisywane do bazy danych aplikacji.
<li><strong>Autoryzacja użytkownika poprzez JSON Web Token</strong> - Każdy użytkownik logujący się do systemu otrzymuje od serwera
wygenerowany token, będący jednoznacznym identyfikatorem użytkownika. Token taki jest zapisywany w pamięci przeglądarki i dodawany
poprzez interceptor do każdego zapytania do serwera. Serwer z kolei, sprawdza istnieje tego tokenu w nagłówku http, sprawdza jego
poprawność,a także czy okres jego ważności nie minął. Na podstawie tego serwer udostępnia zasoby, bądź odsyła użytkownika do
strony logowania w celu potwierdzenia tożsamości.</li>
<li><strong>REST services</strong> - Warstwa frontowa komunikuje się z serwerem za pomocą kilku dostępnych metod.</li>
<li>Single Page Application</strong> - Dzięki wykorzystaniu routingu warstwa frontowa to jedna strona internetowa w sposób dynamiczny
reagująca na zmianę danych</li>
</ul>
<p>Aplikacja pozwala na prowadzenie konwersacji pomiędzy zalogowanymi użytkownikami poprzez grupy. Użytkownik może zasubskrybować
dowolną grupę, jak również ją opuścić</p>
<img src="https://drive.google.com/file/d/11P4XCPJeurNqPidHCUUAlcPtcD5OKFDl/view?usp=sharing" alt="Widok ekranu logowania"/>
<img src="https://drive.google.com/file/d/1bXg2of-10x36Hqev4zz7Gd8_9TCuJq4a/view?usp=sharing" alt="Widok ekranu rejestracji"/>
<img src="https://drive.google.com/file/d/1mxE_Y98YEdEoKTVkxvZVdtHmK8yKqx-l/view?usp=sharing" alt="Widok strony głównej"/>
<img src="https://drive.google.com/open?id=1kToKue2LQrnjhcd5nPzIkiWgY2iSt39O" alt="Widok dodawania grup"/>