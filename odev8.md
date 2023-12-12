# Patika SQL Odev-8

#### 1. *test* veritabanınızda *employee* isimli sütun bilgileri id(INTEGER), name VARCHAR(50), birthday DATE, email VARCHAR(100) olan bir tablo oluşturalım.

````roomsql
CREATE TABLE employee (
	id INT IDENTITY(1,1) PRIMARY KEY,
	emp_name VARCHAR(50) NOT NULL,
	emp_email VARCHAR(100) NOT NULL,
	birthday DATE
);
````

#### 2. Oluşturduğumuz *employee* tablosuna 'Mockaroo' servisini kullanarak 50 adet veri ekleyelim.

````roomsql
insert into employee (emp_name, birthday, emp_email) values ('Zahara Endrici', '2003-01-09', 'zendrici0@apache.org');
insert into employee (emp_name, birthday, emp_email) values ('Leeland Shillum', null, 'lshillum1@psu.edu');
insert into employee (emp_name, birthday, emp_email) values ('Arlana Mirando', null, 'amirando2@sourceforge.net');
insert into employee (emp_name, birthday, emp_email) values ('Letitia Mothersole', '1978-08-19', 'lmothersole3@eventbrite.com');
insert into employee (emp_name, birthday, emp_email) values ('Eryn Andell', '1992-11-29', 'eandell4@nymag.com');
insert into employee (emp_name, birthday, emp_email) values ('Clerc Woodier', null, 'cwoodier5@usnews.com');
insert into employee (emp_name, birthday, emp_email) values ('Cornela Schenkel', '2009-09-29', 'cschenkel6@spotify.com');
insert into employee (emp_name, birthday, emp_email) values ('Mureil Lapham', '1988-11-14', 'mlapham7@cnbc.com');
insert into employee (emp_name, birthday, emp_email) values ('Joannes Mead', null, 'jmead8@japanpost.jp');
insert into employee (emp_name, birthday, emp_email) values ('Orly Hoxey', null, 'ohoxey9@jigsy.com');
insert into employee (emp_name, birthday, emp_email) values ('Kippy Eyckelberg', '1971-06-15', 'keyckelberga@indiegogo.com');
insert into employee (emp_name, birthday, emp_email) values ('Lisha Larroway', null, 'llarrowayb@deliciousdays.com');
insert into employee (emp_name, birthday, emp_email) values ('Glad Klejin', '1986-02-06', 'gklejinc@noaa.gov');
insert into employee (emp_name, birthday, emp_email) values ('Nathanial Shreenan', '1980-02-20', 'nshreenand@wikispaces.com');
insert into employee (emp_name, birthday, emp_email) values ('Alyce Northill', '2001-07-05', 'anorthille@ebay.com');
insert into employee (emp_name, birthday, emp_email) values ('Tye Hapgood', '1989-02-19', 'thapgoodf@simplemachines.org');
insert into employee (emp_name, birthday, emp_email) values ('Darby Barles', '2005-12-27', 'dbarlesg@delicious.com');
insert into employee (emp_name, birthday, emp_email) values ('Neile Yoskowitz', '1992-05-16', 'nyoskowitzh@purevolume.com');
insert into employee (emp_name, birthday, emp_email) values ('Dale Auden', '1979-01-12', 'daudeni@utexas.edu');
insert into employee (emp_name, birthday, emp_email) values ('Ben Pieters', '2006-12-19', 'bpietersj@imageshack.us');
insert into employee (emp_name, birthday, emp_email) values ('Fiona Robbert', '2002-06-11', 'frobbertk@paginegialle.it');
insert into employee (emp_name, birthday, emp_email) values ('Sal Egginton', '2001-11-16', 'seggintonl@51.la');
insert into employee (emp_name, birthday, emp_email) values ('Sashenka Gibbs', '2009-10-15', 'sgibbsm@google.fr');
insert into employee (emp_name, birthday, emp_email) values ('Court Kovacs', '1975-05-11', 'ckovacsn@psu.edu');
insert into employee (emp_name, birthday, emp_email) values ('Vincenz Screase', '1975-10-23', 'vscreaseo@de.vu');
insert into employee (emp_name, birthday, emp_email) values ('Hobard Burchmore', null, 'hburchmorep@godaddy.com');
insert into employee (emp_name, birthday, emp_email) values ('Ginger Pattison', '2003-09-05', 'gpattisonq@clickbank.net');
insert into employee (emp_name, birthday, emp_email) values ('Hestia Pinchbeck', null, 'hpinchbeckr@europa.eu');
insert into employee (emp_name, birthday, emp_email) values ('Anette Edwards', '1989-08-28', 'aedwardss@odnoklassniki.ru');
insert into employee (emp_name, birthday, emp_email) values ('Britni Kembrey', '2008-06-06', 'bkembreyt@miibeian.gov.cn');
insert into employee (emp_name, birthday, emp_email) values ('Leif Mapledoram', '2008-07-23', 'lmapledoramu@51.la');
insert into employee (emp_name, birthday, emp_email) values ('Marrissa Beauvais', '1976-02-05', 'mbeauvaisv@networkadvertising.org');
insert into employee (emp_name, birthday, emp_email) values ('Elyn Lambrecht', null, 'elambrechtw@angelfire.com');
insert into employee (emp_name, birthday, emp_email) values ('Lia Rizzardi', null, 'lrizzardix@friendfeed.com');
insert into employee (emp_name, birthday, emp_email) values ('Madel Vondra', '1988-12-19', 'mvondray@etsy.com');
insert into employee (emp_name, birthday, emp_email) values ('Westbrook Eard', '1998-03-10', 'weardz@craigslist.org');
insert into employee (emp_name, birthday, emp_email) values ('Rosalia Karel', '1977-01-24', 'rkarel10@nsw.gov.au');
insert into employee (emp_name, birthday, emp_email) values ('Marv Carsberg', '2004-07-22', 'mcarsberg11@ning.com');
insert into employee (emp_name, birthday, emp_email) values ('Torey Bresnahan', '1972-04-06', 'tbresnahan12@gmpg.org');
insert into employee (emp_name, birthday, emp_email) values ('Antonius Dakhov', '2010-05-06', 'adakhov13@apache.org');
insert into employee (emp_name, birthday, emp_email) values ('Chelsea Seiter', '1995-06-04', 'cseiter14@google.com.hk');
insert into employee (emp_name, birthday, emp_email) values ('Tabb Collinson', '1976-11-05', 'tcollinson15@php.net');
insert into employee (emp_name, birthday, emp_email) values ('Neddie Coslitt', '1997-09-05', 'ncoslitt16@blogs.com');
insert into employee (emp_name, birthday, emp_email) values ('Worden Schultes', '2001-04-29', 'wschultes17@prnewswire.com');
insert into employee (emp_name, birthday, emp_email) values ('Van Briiginshaw', '1974-09-29', 'vbriiginshaw18@illinois.edu');
insert into employee (emp_name, birthday, emp_email) values ('Rici Ruppelin', '1978-12-09', 'rruppelin19@discovery.com');
insert into employee (emp_name, birthday, emp_email) values ('Jeramey Sketchley', '1979-04-22', 'jsketchley1a@so-net.ne.jp');
insert into employee (emp_name, birthday, emp_email) values ('Ashlen Panyer', '1982-11-08', 'apanyer1b@feedburner.com');
insert into employee (emp_name, birthday, emp_email) values ('Killian Narey', '1984-10-22', 'knarey1c@barnesandnoble.com');
insert into employee (emp_name, birthday, emp_email) values ('Louis Plascott', '1983-09-17', 'lplascott1d@marriott.com');
````
#### 3. Sütunların her birine göre diğer sütunları güncelleyecek 5 adet UPDATE işlemi yapalım.

````roomsql
UPDATE employee 
SET emp_name = 'Elif',
    emp_email = 'elifffk@gmail.com',
    birthday = '1990-12-09'
WHERE id = 1;

UPDATE employee 
SET emp_name = 'Havva',
    emp_email = 'jdfdk@gmail.com',
    birthday = '1992-10-09'
WHERE id = 2;

UPDATE employee 
SET emp_name = 'Aslan',
    emp_email = 'kfjşslkd@gmail.com',
    birthday = '1998-09-09'
WHERE id = 3;

UPDATE employee 
SET emp_name = 'Fatma',
    emp_email = 'elifffk@gmail.com',
    birthday = '1980-12-12'
WHERE id = 4;

UPDATE employee 
SET emp_name = 'Recep',
    emp_email = 'sdjfhd@gmail.com',
    birthday = '1990-01-09'
WHERE id = 5;
````

#### 4. Sütunların her birine göre ilgili satırı silecek 5 adet DELETE işlemi yapalım.

````roomsql
DELETE FROM employee
WHERE id = 1;

DELETE FROM employee
WHERE emp_name = 'Aslan';

DELETE FROM employee
WHERE emp_name = 'RECEP';

DELETE FROM employee
WHERE id = 20;

DELETE FROM employee
WHERE birthday = '1992-10-09';
````
