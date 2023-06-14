# SQL-Bookstore
Using SQL 

SQL Queries: <br>

CREATE DATABASE Bookstore;<br>

USE Bookstore;
CREATE TABLE Books (
    BookID INTEGER,
    Title TEXT,
    Author TEXT,
    PublicationYear INTEGER,
    Price REAL
);<br>

INSERT INTO Books (Title, Author, PublicationYear, Price) VALUES<br>
    ('1','To Kill A Mockingbird', 'Harper Lee', 1960, 12.99),<br>
    ('2','1984', 'George Orwell', 1929, 9.99),<br>
    ('3','Pride and Prejudice', 'Jane Austen', 1813, 8.99),<br>
    ('4','A Court of Thorns and Roses', 'Sarah J Maas', 2015, 10.99),<br>
    ('5','A Court of Mist and Fury', 'Sarah J Maas', 2016, 12.99),<br>
    ('6','A Court of Wings and Ruin', 'Sarah J Maas, 2017, 14.99),<br>
    ('7','A Court of Frost and Starlight', 'Sarah J Maas', 2018, 9.99),<br>
    ('8','A Court of Silver Flames', 'Sarah J Maas', 2021, 16.99); <br>
    
  SELECT * FROM Books;<br>
  SELECT * FROM Books WHERE PublicationYear > 2000;<br>
  SELECT * FROM Books WHERE Author = 'Jane Austen';<br>
  UPDATE Books SET Price = 9.99 WHERE Title = 'Pride and Prejudice';<br>
  DELETE FROM Books WHERE BookID = 4;<br>
  <br>

Learning:
This assignment allowed me to navigate SQL and practice SQL queries to manipulate a table in the Bookstore 
database, which I also had to learn to create. Initially, I faced difficulties connecting to a database to 
start the project. However, I was able to create the basic structure using DB Browser. I am still working on 
effectively using the terminal, so I resorted to using the SQL Editor to run the commands. As I continue 
exploring the features of SQL, I am confident that I will become more comfortable and efficient in using the 
terminal on my device. In the meantime, I am actively exploring and sharing what I have learned with my 
peers, as well as asking their approach to this task.

<br>
<br>
<br>

SQL Query Practice and Database Modification<br>

SQL QUERIES FOR PT 2:<br>
INSERT INTO Books (BookID, Title, Author, PublicationYear, Price) <br>
VALUES <br>
(9, 'The Hidden Path', 'Emma Thonpson',2019, 24.99),<br>
(10, 'Beyond the Horizon', 'Benjamin Richards', 2022, 28.50),<br>
(11, 'Whispering Shadows', 'Olivia Bennet', 2021, 22.95),<br>
(12, 'The Forgotten Tales', 'Nathan Foster', 2023, 21.75),<br>
(13, 'Echos of Eternity', 'Victoria Moore', 2020, 23.99);<br>
<br>
--retreving books costing 20$ or more<br>
<br>
SELECT *<br>
FROM Books<br>
WHERE Price >= 20;<br>
<br>
--retrieving books with publication years between 1980-2020<br>
<br>
SELECT *<br>
FROM Books<br>
WHERE PublicationYear > 1980 AND PublicationYear < 2020;<br>
<br>
--counting books by each author<br>
<br>
SELECT Author, COUNT(*) AS NumberOfBooks<br>
FROM Books<br>
GROUP BY Author;<br>
<br>
--avg price of all books in table<br>
<br>
SELECT AVG(Price) AS AveragePrice<br>
FROM Books;<br>
<br>
--modifying data<br>
<br>
--update price of books published before 1990 by 10%<br>
<br>
UPDATE Books<br>
SET Price = Price * 0.9<br>
WHERE PublicationYear < 1990;<br>
<br>
SELECT * FROM Books;<br>
<br>
--delete books published more than 50 years ago<br>
<br>
DELETE FROM Books<br>
WHERE PublicationYear < CURRENT_DATE - 50;<br>
<br>
SELECT * FROM Books;<br>
<br>
<br>
Learning: I have come to realization that using the command like would be trying to code in a notepad when 
using SQL, thanks, Sher! I am now more confident in using the SQL Editor to run commands to reach a desired 
outcome. I had to do more research on getting the commands to modify the data, and I am glad I got to 
practice retieving data using SELECT, FROM, WHERE and update data using UPDATE, SET, WHERE. I use the 
SELECT * FROM Books after each command to make sure the data is being updated. I also learned how to make 
comments on SQL Editor to help me go back to certain commands and see if I made mistakes. 


