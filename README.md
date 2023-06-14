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

INSERT INTO Books (Title, Author, PublicationYear, Price) VALUES
    ('1','To Kill A Mockingbird', 'Harper Lee', 1960, 12.99),
    ('2','1984', 'George Orwell', 1929, 9.99),
    ('3','Pride and Prejudice', 'Jane Austen', 1813, 8.99),
    ('4','A Court of Thorns and Roses', 'Sarah J Maas', 2015, 10.99),
    ('5','A Court of Mist and Fury', 'Sarah J Maas', 2016, 12.99),
    ('6','A Court of Wings and Ruin', 'Sarah J Maas, 2017, 14.99),
    ('7','A Court of Frost and Starlight', 'Sarah J Maas', 2018, 9.99),
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



