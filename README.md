[//]: # (About the Project)
## :star2: About the Project

This Inventory management system is the currently Ford Asia Pacific after-sales logistics warehousing supply chain process.
After I leave Ford, I start this project in order to help some who need it. 
OneAPP Type. Support scanner PDA, mobile APP, desktop exe, website as well.

[//]: # (Function)
## :dart: Function

* [x] Multiple Warehouses
* [x] Supplier Management
* [x] Customer Management
* [x] Scanner PDA
* [x] Cycle Count
* [x] Order Management
* [x] Stock Control
* [x] Safety Stock Show
* [x] API Documents
* [x] IOS APP Support
* [x] Android APP Support
* [x] Electron APP Support
* [x] Auto Update
* [x] i18n Support
* [x] API Documents

[//]: # (Install)
## :compass: Install
Python install
- [python 3.8.10](https://www.python.org/downloads/release/python-3810/)

Nodejs install
- [nodejs 14.19.3](https://nodejs.org/download/release/v14.19.3/)

Twisted install
- Please google how to install Twisted , if you have some problem on install it . 

### docker(Optional)
~~~shell
cd GreaterWMS/
docker-compose up -d
# Change Baseurl
# baseurl GreaterWMS/templates/public/statics/baseurl.txt
docker-compose restart
~~~

[//]: # (development)
## :hammer_and_wrench: How To Run Development Server:

- Run Backend:
~~~shell
cd GreaterWMS
daphne -p 8008 greaterwms.asgi:application
or
daphne -b 0.0.0.0 -p 8008 greaterwms.asgi:application # lan
~~~

- Run Frontend:
~~~shell
cd templates
quasar d
~~~

- Change Request Baseurl
~~~shell
templates/public/statics/baseurl.txt
~~~

- API Documents

~~~shell
baseurl + '/docs/'
~~~

### Companion Mobile APP

- App Source Code

~~~shell
npm install cordova -g

cd app
yarn install
## Development
quasar d -m cordova -T [android, ios]
## Deploy
quasar build -m [android, ios]
~~~

- You can directly use app if you don't want to build it 

[//]: # (publish)
## :trumpet: How To Publish Your APP:

- Web Build:

~~~shell
cd templates
quasar build
~~~

[//]: # (deploy)
## :computer: How To Deploy Server:

If the server has SSL enabled, please use HTTPS and WSS, if SSL is not enabled, use HTTP and WS

The front-end code needs to be rebuilt after modification.