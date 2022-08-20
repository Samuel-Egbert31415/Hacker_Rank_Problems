Given the CITY and COUNTRY tables, query the sum of the populations of all cities where the CONTINENT is 'Asia'.

Note: CITY.CountryCode and COUNTRY.Code are matching key columns.

Input Format

The CITY and COUNTRY tables are described as follows:
![img_1.png](img_1.png)
![img_2.png](img_2.png)

SELECT SUM(Ct.POPULATION) \
FROM CITY Ct \
INNER JOIN COUNTRY Co \
ON Ct.COUNTRYCODE = Co.CODE \
WHERE Co.CONTINENT = 'Asia';