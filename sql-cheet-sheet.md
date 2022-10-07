### SQL cheet sheet 

```
1.CREATE DATABASE DatabaseName;
2.DROP DATABASE DatabaseName;
3.USE DatabaseName;
4. create table TableName(
    -> id int(11) not null auto_increment,
    -> name varchar(234) not null,
    -> age varchar(344) not null,
    -> email varchar(45) not null,
    -> primary key(id)
    -> );
5.DROP TABLE TableName;
6.
7.ALTER TABLE TableName ADD(
		->roll int(11) not null,
		->shift varchar(50) not null
		->);
8.ALTER TABLE TableName MODIFY(
		->roll varchar(5000) not null,
		->shift varchar(100) not null
		->);
9.RENAME Old_table TO New_table;
10.INSERT INTO TableName(name,roll,shift) VALUES ('faisal','23466','first');
11.UPDATE TableName SET name="sharia emon faisal",roll="456" where id=1;
12.INSERT INTO TableName(name,roll,shift) VALUES ('Sharia','382334','Morning Shift');
13.SELECT * FROM TableName;
14.SELECT * FROM TableName WHERE id=5;
15.SELECT * FROM TableName;
16.SELECT id,name,roll FROM TableName;
17.UPDATE TableName SET name='Faisal',roll='45667' WHERE id=3;
18.DELETE FROM TableName WHERE id=5;
19.SELECT Name FROM TableName;
20.SELECT DISTINCT(roll) FROM tableName;
21.SELECT * FROM WHERE age>25;
22.SELECT * FROM TableName WHERE name='sharia' and roll='382334';  
23.SELECT * FROM TableName  WHERE name='sharia' or roll='382334'; 
24.SELECT * FROM TableName  WHERE name='sharia' and roll='382334'; 
25.SELECT * FROM TableName ORDER BY id ASEC;
26.SELECT * FROM TableName ORDER BY id DESC;
27.SELECT * FROM TableName ORDER BY id;
28.SELECT * FROM TableName LIMIT 5;
29.SELECT * FROM TableName WHERE name LIKE "%something%";
30.SELECT * FROM TableName WHERE name LIKE "something%";
31.SELECT * FROM TableName WHERE name LIKE "%something";
32.SELECT * FROM TableName WHERE name LIKE "someth_ng";
33.SELECT * FROM TableName WHERE name NOT LIKE "%something%";
34.SELECT * FROM TableName WHERE id BETWEEN 5 TO 10; 
35.SELECT * FROM TableName WHERE id NOT BETWEEN 5 TO 10
36.SELECT * FROM TableName WHERE id IN ('3','7');
38.SELECT AVG(age) AS NewVAriable FROM TableName;
39.SELECT max(age) AS NewVAriable FROM TableName;
40.SELECT min(age) AS NewVAriable FROM TableName;
41.SELECT count(age) AS NewVAriable FROM TableName;
42.SELECT sum(age) AS NewVAriable FROM TableName;
43.SELECT UPPER(name) AS NewVariable FROM TableName;
44.SELECT LOWER(name) AS NewVariable FROM TableName;
45.SELECT * FROM Table1 t1 JOIN Tble2 t2 ON t1.st_id=t2.st_id;
46.SELECT * FROM Table1 t1 LEFT JOIN Tble2 t2 ON t1.st_id=t2.st_id;
47.SELECT * FROM Table1 t1 RIGHT JOIN Tble2 t2 ON t1.st_id=t2.st_id;

48. select tbl_product.*, tbl_category.catName, tbl_brand.brandName
    -> from tbl_product
    -> inner join tbl_category on
    -> tbl_product.catId = tbl_category.catId
    -> inner join tbl_brand
    -> on tbl_product.brandId = tbl_brand.brandId
    -> order by tbl_product.proId desc;

or 

=> SELECT p.*,c.catName,b.brandName
     -> FROM tbl_product as p, tbl_category as c, tbl_brand as b
     ->WHERE p.catId = c.catId AND p.brandId = b.brandId
     -> ORDER BY p.proId DESC;

```


