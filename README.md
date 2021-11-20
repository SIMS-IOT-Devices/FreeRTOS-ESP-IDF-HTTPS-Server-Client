# HTTPS-ESP-IDF-Server-Client
ESP IDF HTTPS server and client on the same esp32 in parallel

In order to create the PEM certificates use following OpenSSL commands:
Server PEM certificates:
openssl req -newkey rsa:2048 -nodes -keyout ServerKey.pem -x509 -days 3650 -out ServerCert.pem -subj "/CN=ESP32 HTTPS server"

Client PEM certificates, show all three needed certificates (created specifically for firebase url) on the screen. Copy them to one file:
openssl s_client -showcerts -connect console.firebase.google.com:443
