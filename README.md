# 🚀 Dockerized Node.js Backend with Nginx Reverse Proxy and HTTPS 

This project demonstrates a fully configured web server stack featuring:
- **Node.js backend servers** running in **Dockerized instances**.
- An **Nginx reverse proxy** to load balance traffic across backend servers.
- A secure HTTPS connection to the Nginx proxy using a **self-signed TLS certificate**.

![Untitled](https://github.com/user-attachments/assets/feb320fd-2edd-4890-9e59-1913949f2487)


---

## 🛠️ Features

- **Scalable Backend**: Dockerized Node.js backend servers ensure portability and consistency.
- **Efficient Traffic Management**: Nginx as a reverse proxy load balances requests for optimal performance.
- **Secure Communication**: HTTPS enabled with a self-signed TLS certificate for encrypted connections.

---

## 🚀 Commands & Setup Instructions

### Setting Up SSL with a Self-Signed Certificate

To enable HTTPS for your Nginx reverse proxy, follow these steps:

``
openssl req -x509 -nodes -days 365 -newkey rsa:2048 \
  -keyout nginx-selfsigned.key -out nginx-selfsigned.crt
``

Write your SSL certificate and key in nginx.conf file
