1. The start screen in WinCC Unified must contain a button with name "Logout" (Text can be anything) and a left mouse click event with system function "LogOff"
2. Copy login.html to C:\Program Files\Siemens\Automation\WinCCUnified\WebRH\public
3. Call https://winccunified/WebRH/login.html?user=Otto&password=mypassword and replace the user "Otto" and the password "mypassword" with your credentials.

The website (login.html) tries to login with the given credentials every 500ms. After 30s it stops trying, because maybe no login is needed or the network is down.