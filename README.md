<font color="green">**#[CREATING 2 TABLES AND CONNECTING IT WITH A NEW TABLE THROUGH VARIOUS REFERENCES]**</font>

*First i am creating a table florist that contains item id ,item name, price and its description*

#syntax for the table florist 

please note details such as primary keys, foreign keys, data type, not null constraints

* create table florist(itemid varchar(10) primary key not null, itemnm varchar(15),price int not null, descr varchar(30))
* insert into florist values('GAR','GARLAND',500,' GARLAND OF FRESH MIX ROSES')
* INSERT INTO florist values('BOUQ','BOUQUET',750,'MIX WITH ROSES AND TULIPS')
* INSERT INTO florist values('STI','STICK',1000,'SINGLE STICK OF ORCHID')
* INSERT INTO florist values('GAR.R','GARLAND',2000,'GARLAND OF ROSES')
* INSERT INTO florist values('BOUQ.WO','BOUQUET',750,'BOUQUET OF WHITE ORCHIDS')
* INSERT INTO florist values('STIK.DAND','STICK',750,'STICK OF DANDELIONS')
* INSERT INTO florist values('BOUQ.SUN','BOUQUET',750,'FRESH GROUP OF SUNFLOWERS')

  After execution of the following lines sql creates a table given below

![Florist table](https://github.com/user-attachments/assets/622d468d-2aba-47cb-b379-0f077b554eef)

*NOW*
*I AM CREATING ANOTHER TABLE WHICH WILL CONTAIN  CUSTOMER ID AND CUSTOMER NAME*

#Syntax for the same will be again(please notes the syntax i am using )

* CREATE TABLE CUSTOMER(custid int primary key not null,customernm varchar(20))
* insert into customer values(001,'HARSHIT')
* insert into customer values(002,'NAMAN')
* insert into customer values(003,'PIYUSH')
* insert into customer values(004,'VANSH')
* insert into customer values(005,'KARTIK')




