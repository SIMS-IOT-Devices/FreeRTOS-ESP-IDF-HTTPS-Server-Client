# HTTPS-ESP-IDF-Server-Client
ESP IDF HTTPS server and client on the same esp32 in parallel

In order to create the PEM certificates for server side use following OpenSSL command:

openssl req -newkey rsa:2048 -nodes -keyout ServerKey.pem -x509 -days 3650 -out ServerCert.pem -subj "/CN=ESP32 HTTPS server"


The attached OpenSSL command shows client PEM certificates on the screen. Three certificates (created specifically for firebase url) have to be copied to one file ClientCert.pem.

openssl s_client -showcerts -connect console.firebase.google.com:443
