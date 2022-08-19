Query the list of CITY names from STATION which have vowels (i.e., a, e, i, o, and u) as both their first and last characters. Your result cannot contain duplicates.

Input Format

The STATION table is described as follows:

![img.png](img.png)

where LAT_N is the northern latitude and LONG_W is the western longitude.


SELECT DISTINCT CITY \
FROM STATION \
WHERE CITY REGEXP '^a|^e|^i|^o|^u' \
AND CITY REGEXP 'a$|e$|i$|o$|u$'; 

