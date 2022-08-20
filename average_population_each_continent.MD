Given the CITY and COUNTRY tables, query the names of all the continents (COUNTRY.Continent) and their respective average city populations (CITY.Population) rounded down to the nearest integer.

Note: CITY.CountryCode and COUNTRY.Code are matching key columns.

Input Format

The CITY and COUNTRY tables are described as follows:

![img_5.png](img_5.png)
![img_6.png](img_6.png)

SELECT Co.CONTINENT, FLOOR(AVG(Ct.POPULATION)) as Average_City_Pop \
FROM CITY Ct \
INNER JOIN COUNTRY Co \
ON Ct.COUNTRYCODE = Co.CODE \
GROUP BY Co.Continent;