# MysqlAssesment

insert into Movies Values ('When they See us', 121, 'Drama', 5.0, 'R');
Query OK, 1 row affected (0.02 sec)

mysql> insert into Movies Values ('Transformers', 119, 'Action', 4.9, 'R');
Query OK, 1 row affected (0.00 sec)

 Select title from Movies where genre = 'Sci-Fi';
 Select title from Movies where IMDscore >= 6.5;
 select title from movies where rating in ('g', 'PG') and runtime < 100;
 select genre, AVG(runtime) as Average_runtime from Movies where IMDscore < 7.5 group by genre order by genre;
 UPDATE Movies set rating = 'R' where title = 'Starship Troopers';
 select rating, AVG(IMDscore) as Average_Score, Min(IMDscore) as Min_Score, MAX(IMDscore) as Max_Score from Movies group by rating order by rating;
 
