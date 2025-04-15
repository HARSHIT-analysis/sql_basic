# PROJECT SQL BASIC :
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

#Syntax for the same IS given below {again(please notes the syntax i am using)}

* CREATE TABLE CUSTOMER(custid int primary key not null,customernm varchar(20))
* insert into customer values(001,'HARSHIT')
* insert into customer values(002,'NAMAN')
* insert into customer values(003,'PIYUSH')
* insert into customer values(004,'VANSH')
* insert into customer values(005,'KARTIK')

![CUSTOMER TABLE](https://github.com/user-attachments/assets/a624f35e-388c-4989-9753-eb2c288da2df)

 the third table is going to be the order of the customer and it will contain orderno, item id  from florist table, customer id from customer table, order quantity,and the date  of the order .
 * down below are the syntaxes where in i have created the columns then again added some more columns using alter and then made some changes to touch an imp aspect of sql
   filteration using where to give reference to make changes in the respective columns.
   
* CREATE TABLE ORDERNO(orderno int not null, Itemid varchar(10) references florist(itemid) ,Custid int references CUSTOMER(custid))
* select * from ORDERNO
* alter TABLE ORDERNO ADD orderqt int not null,orderdt date default getdate()
* insert into ORDERNO values(101,'BOUQ.SUN',004,3,getdate())
* insert into ORDERNO values(102,'GAR.R',004,9,getdate())
* insert into ORDERNO values(103,'STIK.DAND',004,3,getdate())
* insert into ORDERNO values(104,'BOUQ',003,5,getdate())
* insert into ORDERNO values(105,'GAR',002,8,getdate())
* insert into ORDERNO values(106,'GAR.R',005,4,getdate())
* UPDATE ORDERNO set orderno=111 where Itemid='GAR.R'
  
  *HERE GOES THE FINAL OUTPUT TABLE USING BOTH THE ABOVE TABLES AS A REFERENCE*

  ![ORDER OF THE CUSTOMERS](https://github.com/user-attachments/assets/fd1a0e91-e65e-49bc-af92-8c2de98d4274)





