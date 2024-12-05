URL repozitorija : https://github.com/BABYDUXY/appb-dg.git

sql upit - prikazati broj knjiga za određenoga autora:
SELECT COUNT(naslov),autor.prezime_ime
FROM knjiga
INNER JOIN autor ON knjiga.autor=autor.id
WHERE autor.prezime_ime="Josip Kozarac"
GROUP BY autor.id
