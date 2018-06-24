# SMTP
#
# Este projeto tem a finalidade de mostrar como enviar um email autenticado via Telnet
# 23/06/2018

Comandos via shell TELNET

> telnet smtp.rjc.com.br 587

HELO smtp.rjc.com.br

AUTH LOGIN        // o servidor irá perguntar o usuario e senha em codificação base 64 bits

Y29tZXJjaWFsQHJqYy5jb20uYnI=  // comercial@rjc.com.br

cmRhbEBtdWRhcjIwMTg=          // 123456

MAIL FROM: <comercial@rjc.com.br> // usar <> com email dentro

RCPT TO: <robisonjunior@gmail.com>  // usar <> com email dentro

DATA

From: "God at Heaven" <comercial@rjc.com.br>
To: "Robison Junior" <robisonjunior@gmail.com>
Subject: Just a test message
This is just a test message from God.
Bye.
God at Heaven
.

quit

site conversor 64 bits : https://4devs.com.br/codificar_decodificar_base64
