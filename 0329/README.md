�إ�...
* ��Ʈw test0329
* ��ƪ�table moneybook
* ���
	m_id    Primary key
	name    200�H�U���r��
	cost    ���
	
�إ�..�i�H�ާ@�o�Ӹ�Ʈw���ϥΪ� mememe / 123456

1. ���� D:\xampp\mysql\bin\mysql -uroot
2. �ϥ� http://localhost/phpmyadmin/
3. �ϥ� adminer
   http://localhost/adminer.php
   

�R�O���ܦr�� D:\xampp\mysql\bin\mysql -uroot

````
CREATE DATABASE test0329 DEFAULT CHARACTER SET 'utf8' DEFAULT COLLATE 'utf8_general_ci';

CREATE USER 'mememe'@'localhost' IDENTIFIED BY '123456';

GRANT ALL PRIVILEGES ON test0329.* TO 'mememe'@'localhost';

FLUSH PRIVILEGES;

EXIT;
````

�R�O���ܦr�� D:\xampp\mysql\bin\mysql -umememe -p

````
USE test0329;

CREATE TABLE moneybook (
  m_id INT UNSIGNED NOT NULL AUTO_INCREMENT PRIMARY KEY,
  name VARCHAR(200),
  cost INT
) CHARACTER SET 'utf8' COLLATE 'utf8_general_ci';
````
