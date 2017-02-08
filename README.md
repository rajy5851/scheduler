### Flask + fullcalendar Sample
----------------------------
- install python 2.7
- install mysql
- create database
- create table

```sql
CREATE TABLE `my_schedule` (
  `id` int(11) NOT NULL AUTO_INCREMENT,
  `title` varchar(255) NOT NULL,
  `start` datetime NOT NULL,
  `end` datetime NOT NULL,
  `allDay` char(1) NOT NULL DEFAULT 'Y',
  PRIMARY KEY (`id`)
)
```

- clone project

```
$ git clone git@github.com:ParkMinKyu/scheduler.git
```

- install [virtualenv](https://virtualenv.pypa.io/en/stable/)

```
$ sudo pip install virtualenv
```

- create virtualenv && activate

```
$ virtualenv envname
$ . envname/bin/activate
(envname) $
```

- install flask && pymysql

```
(envname) $ pip install flask
(envname) $ pip install pymysql
```

- run application

```
(envname) $ python application.py
```
