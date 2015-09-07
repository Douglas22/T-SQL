# T-SQL
/*
useing tabe customers witch has 6 columbs and some nulls in the 6th 
sepret querys rather than one long one
*/
select *
from customers
where ID like ('2%')



select count(*)
from customers
where ID like ('2%')

select *
from customers
where spent is null


select *
from (select ID , lname, fname , Address , phonenumber,spent
FROM customers 
where ID = '123' ) as d



select *
from (select ID , lname, fname , Address , phonenumber,spent
FROM customers 
where ID = '123' ) as d
where spent is null


select *
from customers
where spent is null 
select rtrim('phonenumber')

select count(*)
from customers
where ID like '1%'

select count(*)
from customers
where len(phonenumber)>3

select *
from customers
select left('phonenumber',3)
select REPLACE('banks','b','z')
