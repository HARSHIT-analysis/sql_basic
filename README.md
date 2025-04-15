<font color="green">**#[CREATING 2 TABLES AND CONNECTING IT WITH A NEW TABLE THROUGH VARIOUS REFERENCES]**</font>

*First i am creating a table florist that contains item id ,item name, price and its description*

#syntax for the table florist 

* create table florist(itemid varchar(10) primary key not null, itemnm varchar(15),price int not null, descr varchar(30))
* insert into florist values('GAR','GARLAND',500,' GARLAND OF FRESH MIX ROSES')
* INSERT INTO florist values('BOUQ','BOUQUET',750,'MIX WITH ROSES AND TULIPS')
* INSERT INTO florist values('STI','STICK',1000,'SINGLE STICK OF ORCHID')
* INSERT INTO florist values('GAR.R','GARLAND',2000,'GARLAND OF ROSES')
* INSERT INTO florist values('BOUQ.WO','BOUQUET',750,'BOUQUET OF WHITE ORCHIDS')
* INSERT INTO florist values('STIK.DAND','STICK',750,'STICK OF DANDELIONS')
* INSERT INTO florist values('BOUQ.SUN','BOUQUET',750,'FRESH GROUP OF SUNFLOWERS')

![Florist table](https://github.com/user-attachments/assets/622d468d-2aba-47cb-b379-0f077b554eef)



