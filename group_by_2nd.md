2. Contare gli insegnanti che hanno l'ufficio nello stesso edificio

SELECT COUNT(*) as `number_teachers`, `office_address` 

FROM `teachers` 

GROUP BY `office_address`;
