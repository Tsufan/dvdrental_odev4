# dvdrental_odev4
patika.dev dvdrental örnek veri tabanı ile sorgular ödev4


1)film tablosunda bulunan replacement_cost sütununda bulunan birbirinden farklı değerleri sıralayınız.
```
SELECT DISTINCT replacement_cost FROM film;
```
![1](sorgu_1.png)
***
2)film tablosunda bulunan replacement_cost sütununda birbirinden farklı kaç tane veri vardır?
```
SELECT COUNT(DISTINCT replacement_cost) FROM film;
```
![2](sorgu_2.png)
***
3)film tablosunda bulunan film isimlerinde (title) kaç tanesini T karakteri ile başlar ve aynı zamanda rating 'G' ye eşittir?
```
SElECT COUNT(*) FROM film
WHERE title LIKE 'T%'
AND rating = 'G';
```
![3](sorgu_3.png)
***

4)country tablosunda bulunan ülke isimlerinden (country) kaç tanesi 5 karakterden oluşmaktadır?
```
SElECT COUNT(*) FROM country
WHERE country LIKE '_____'
```
![4](sorgu_4.png)
***

5)city tablosundaki şehir isimlerinin kaçtanesi 'R' veya r karakteri ile biter?
```
SElECT COUNT(*) FROM city
WHERE city ILIKE '%r';
```
![5](sorgu_5.png)