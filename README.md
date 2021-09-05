# SQL_ODEV4
**Patika SQL eğitimi kapsamında yaptığım ödev4**
-
1._film tablosunda bulunan replacement_cost sütununda bulunan birbirinden farklı değerleri sıralayınız._
```sql
SELECT DISTINCT(replacement_cost) FROM film;
```
2._film tablosunda bulunan replacement_cost sütununda birbirinden farklı kaç tane veri vardır?_
```sql
SELECT COUNT(DISTINCT(replacement_cost)) FROM film;
```
3._film tablosunda bulunan film isimlerinde (title) kaç tanesini T karakteri ile başlar ve aynı zamanda rating 'G' ye eşittir?_
```sql
SELECT COUNT(*) FROM film WHERE title LIKE 'T%' AND  rating = 'G';
```
4._country tablosunda bulunan ülke isimlerinden (country) kaç tanesi 5 karakterden oluşmaktadır?_
```sql
SELECT COUNT(*) FROM country WHERE country LIKE '_____';
```
5._city tablosundaki şehir isimlerinin kaçtanesi 'R' veya r karakteri ile biter?_
```sql
SELECT COUNT(*) FROM city WHERE city ILIKE '%r';
```
---------
Sorgu senaryolarını [dvdrental.tar](https://www.postgresqltutorial.com/wp-content/uploads/2019/05/dvdrental.zip) isimli dosyayı indirerek gerçekleştirebilirsiniz.

