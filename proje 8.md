SQL > Ödev 8
www.patika.dev


1-) test veritabanınızda employee isimli sütun bilgileri id(INTEGER), name VARCHAR(50), birthday DATE, email VARCHAR(100) olan bir tablo oluşturalım.

CREATE TABLE employee (
	id INT,
	name VARCHAR(50),
	birthday DATE,
	email VARCHAR(100)
);

2-) Oluşturduğumuz employee tablosuna 'Mockaroo' servisini kullanarak 50 adet veri ekleyelim.

insert into employee (id, name, email, birthday) values (1, 'Randene', 'rgabe0@fema.gov', '1919-08-13');

............
............
............

insert into employee (id, name, email, birthday) values (50, 'Diana', 'daizikov1d@geocities.jp', '1948-01-19');

3-) Sütunların her birine göre diğer sütunları güncelleyecek 5 adet UPDATE işlemi yapalım.

UPDATE employee
SET name = 'Mustafa',
	birthday = '1994-07-07'
WHERE id = 2

4-) Sütunların her birine göre ilgili satırı silecek 5 adet DELETE işlemi yapalım.

DELETE FROM employee
WHERE name = 'Mustafa'
