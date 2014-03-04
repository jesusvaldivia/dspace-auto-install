dspace-auto-install
===================

Automatic install DSpace on Ubuntu like systems

This project was based in article LiveCD on [Wiki DSpace].

Download a Linux Image
----------------------

Para evitar o processo de instalação do Linux foi baixada uma imagem do XUbuntu, localizada no site [Virtual Box Images], conforme abaixo:

**Xubuntu 12.04 codename Precise Pangolin**

Size (compressed/uncompressed): 502.2 MBytes / 2.6 GBytes

[XUbuntu Image]

Active user account(s) (username/password): xubuntu/reverse

Clone the repository
--------------------

Criei um arquivo contendo os arquivos necessários para a instalação do DSpace sem quase nenhuma intervenção “manual”, clone o repositório na pasta /home/xubuntu/dspace (por exemplo)

Change the parameters
---------------------

Altere os parâmetros dos arquivos abaixo de acordo com suas necessidades:

build-dspace
------------

VERSION_DSPACE="4.1"

build.properties
------------

dspace.name = DSpace

default.language = pt_BR

dspace.cfg
------------

dspace.name = DSpace

default.language = pt_BR

mail.server=smtp.gmail.com

mail.server.username = treinamento.dspace@gmail.com

mail.server.password = yourPassword

mail.extraproperties = mail.smtp.socketFactory.port=465, \

mail.smtp.socketFactory.class=javax.net.ssl.SSLSocketFactory, \

mail.smtp.socketFactory.fallback=false

mail.from.address = treinamento.dspace@gmail.com

feedback.recipient = treinamento.dspace@gmail.com

mail.admin = treinamento.dspace@gmail.com

alert.recipient = treinamento.dspace@gmail.com

registration.notify = treinamento.dspace@gmail.com

Install
-------

cd /home/xubuntu/dspace

./build-dspace


[Virtual Box Images]:"http://virtualboxes.org/images/ubuntu/"
[Wiki DSpace]:"https://wiki.duraspace.org/display/DSPACE/LiveCD"
[XUbuntu Image]:"http://downloads.sourceforge.net/virtualboximage/xubuntu_1204.7z"
