 8. Quanti sono gli insegnanti che non hanno un numero di telefono? (50)
    SELECT COUNT(*) AS 'insegnanti senza numero di telefono' FROM `teachers` WHERE `phone`IS NULL;
