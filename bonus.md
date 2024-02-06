Selezionare nome, descrizione e periodo di tutti i corsi che hanno sito web diverso da null, cfu compresi tra 9 e 12 e che sono del primo anno ed ordinarli in ordine decrescente

SELECT `name`,`description`,`period` 
FROM `courses` 
WHERE `website` IS NOT NULL 
AND `cfu` BETWEEN '9' AND '12' 
AND `year`= '1' 
ORDER BY `cfu` DESC;
