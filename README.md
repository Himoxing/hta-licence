POLISH/ENGLISH DOCUMENTATION:

Documentation English: License System Application
Overview
The "License System" application is a simple HTML-based application designed to provide a login mechanism and a dashboard for authorized users. It utilizes the HTA (HTML Application) framework and includes VBScript for handling user authentication and navigation between different sections of the application. The application's primary purpose is to allow users to log in and access a dashboard with various functionalities.

Application Components
The application consists of several components, including HTML, VBScript, and CSS, that work together to create the user interface and functionality.

HTML Structure
The HTML structure defines the layout and content of the application's interface. It includes the following key elements:

<head>: Contains metadata and script references.

<title>: Specifies the title of the application.
<HTA:APPLICATION>: Configures HTA-specific properties such as the application name, window behavior, and more.
<script>: Contains VBScript code for handling user interactions and data processing.

checkLogin(): Validates user login credentials against stored data from an external source (login_data.txt).
SwitchToDashboard(): Switches the view from the login container to the dashboard container upon successful login.
Logout(): Logs the user out and switches back to the login container.
<body>: Contains the main content of the application.

<div id="loginContainer">: Represents the login interface.

<input type="text"> and <input type="password">: Fields for entering the login credentials.
<button onclick="checkLogin()">: Initiates the login process.
<div id="dashboardContainer">: Represents the dashboard interface.

<button onclick="Logout()">: Initiates the logout process.
VBScript Functions
The VBScript functions provide the core functionality of the application:

checkLogin(): Responsible for authenticating user credentials and displaying appropriate messages.

Retrieves the user's entered login and password.
Sends an HTTP GET request to an external source (https://example.com/login_data.txt) to retrieve stored login data.
Compares entered credentials with stored data.
If authenticated, switches to the dashboard view.
If authentication fails, displays an error message.
SwitchToDashboard(): Handles switching the view from the login interface to the dashboard interface.

Hides the login container and displays the dashboard container.
Logout(): Handles the logout process by clearing the logged-in state and switching back to the login interface.

Resets the loggedIn flag to False.
Hides the dashboard container and displays the login container.
Usage
Open the application in an HTML-capable browser or double-click the file to run it as an HTA application.
The login container is initially displayed.
Enter valid login credentials and click the "login" button.
If authenticated, the dashboard container will be displayed, allowing access to various functionalities.
Click the "logout" button in the dashboard to log out and return to the login container.
Notes
The application is intended for educational purposes and provides basic login functionality. In a real-world scenario, security considerations such as hashing and encryption should be implemented for storing and transmitting credentials.
The application references an external source (https://example.com/login_data.txt) for login data. In practice, this should be replaced with a secure and properly structured backend for managing user data.
HTA applications might have compatibility limitations in modern browsers, and security concerns should be addressed when using this technology.
Disclaimer: This documentation is for explanatory purposes only and does not cover security best practices, design considerations, or full application development details.


DOCUMENTATION POLISH:

Dokumentacja: Aplikacja Systemu Licencjonowania
Przegląd
Aplikacja "System Licencjonowania" to prosta aplikacja oparta na strukturze HTML, która ma za zadanie dostarczyć mechanizm logowania oraz panel sterowania dla autoryzowanych użytkowników. Wykorzystuje ona framework HTA (HTML Application) i zawiera skrypt w języku VBScript, który obsługuje uwierzytelnianie użytkowników oraz nawigację pomiędzy różnymi sekcjami aplikacji. Głównym celem aplikacji jest umożliwienie użytkownikom zalogowania się i uzyskania dostępu do panelu sterowania z różnymi funkcjonalnościami.

Składniki Aplikacji
Aplikacja składa się z kilku elementów, takich jak HTML, VBScript oraz CSS, które współdziałają, tworząc interfejs użytkownika i funkcjonalność.

Struktura HTML
Struktura HTML definiuje układ i zawartość interfejsu aplikacji. Zawiera ona następujące kluczowe elementy:

<head>: Zawiera metadane oraz odniesienia do skryptów.

<title>: Określa tytuł aplikacji.
<HTA:APPLICATION>: Konfiguruje właściwości specyficzne dla frameworka HTA, takie jak nazwa aplikacji, zachowanie okna i inne.
<script>: Zawiera kod w języku VBScript, który obsługuje interakcje użytkownika oraz przetwarzanie danych.

checkLogin(): Weryfikuje dane uwierzytelniania użytkownika w oparciu o dane przechowywane w zewnętrznym źródle (login_data.txt).
SwitchToDashboard(): Przełącza widok z kontenera logowania na kontener panelu sterowania po pomyślnym zalogowaniu.
Logout(): Wylogowuje użytkownika i powraca do kontenera logowania.
<body>: Zawiera główną treść aplikacji.

<div id="loginContainer">: Reprezentuje interfejs logowania.

<input type="text"> oraz <input type="password">: Pola umożliwiające wprowadzenie danych uwierzytelniania.
<button onclick="checkLogin()">: Inicjuje proces logowania.
<div id="dashboardContainer">: Reprezentuje interfejs panelu sterowania.

<button onclick="Logout()">: Inicjuje proces wylogowywania.
Funkcje w języku VBScript
Funkcje napisane w języku VBScript dostarczają podstawową funkcjonalność aplikacji:

checkLogin(): Odpowiada za uwierzytelnianie danych logowania użytkownika oraz wyświetlanie odpowiednich komunikatów.

Pobiera wprowadzony login i hasło użytkownika.
Wysyła zapytanie HTTP GET do zewnętrznego źródła (https://example.com/login_data.txt), aby pobrać przechowywane dane logowania.
Porównuje wprowadzone dane z danymi przechowywanymi.
Jeśli uwierzytelnienie powiedzie się, przełącza widok na panel sterowania.
Jeśli uwierzytelnienie nie powiedzie się, wyświetla komunikat błędu.
SwitchToDashboard(): Odpowiada za przełączanie widoku z interfejsu logowania na interfejs panelu sterowania.

Ukrywa kontener logowania i wyświetla kontener panelu sterowania.
Logout(): Odpowiada za proces wylogowywania poprzez wyczyszczenie stanu zalogowania i powrót do interfejsu logowania.

Resetuje flagę loggedIn na wartość False.
Ukrywa kontener panelu sterowania i wyświetla kontener logowania.
Użycie
Otwórz aplikację w przeglądarce obsługującej HTML lub dwukrotnie kliknij plik, aby uruchomić ją jako aplikację HTA.
Kontener logowania jest początkowo wyświetlany.
Wprowadź poprawne dane logowania i kliknij przycisk "login".
Jeśli uwierzytelnienie przebiegnie pomyślnie, zostanie wyświetlony kontener panelu sterowania, umożliwiający dostęp do różnych funkcjonalności.
Kliknij przycisk "logout" w panelu sterowania, aby się wylogować i wrócić do kontenera logowania.
Uwagi
Aplikacja jest przeznaczona wyłącznie do celów edukacyjnych i zapewnia podstawową funkcjonalność logowania. W rzeczywistym środowisku należy uwzględnić kwestie związane z bezpieczeństwem, takie jak hashowanie i szyfrowanie, przy przechowywaniu i przesyłaniu danych uwierzytelniania.
Aplikacja odwołuje się do zewnętrznego źródła (https://example.com/login_data.txt) w celu pobrania danych logowania. W praktyce należy to zastąpić bezpiecznym i odpowiednio strukturyzowanym backendem do zarządzania danymi użytkowników.
Aplikacje HTA mogą mieć ograniczenia związane z kompatybilnością w nowoczesnych przeglądarkach, a także należy uwzględnić kwestie związane z bezpieczeństwem podczas korzystania z tej technologii.
Ostrzeżenie: Ta dokumentacja ma charakter wyłącznie wyjaśniający i nie obejmuje najlepszych praktyk z zakresu bezpieczeństwa, koncepcji projektowych ani pełnych szczegółów dotyczących tworzenia aplikacji.
