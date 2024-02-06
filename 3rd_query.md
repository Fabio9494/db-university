3. Selezionare tutti gli studenti che hanno più di 30 anni
SELECT * FROM students WHERE TRUNCATE(DATEDIFF(CURDATE(), `date_of_birth`)/365, 0) > 30;
