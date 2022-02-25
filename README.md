# MachineLearning
building machine learning models that can generate prediction for a total gain/day to a Translation desck_Office, i get the data from an Application_data_base witch i devolopped with a Laravel_FrameWorck; i get the rows by executing the SQL command via PHPMYADMIN by:

SELECT DATE(traductions.created_at) as date,DAYNAME(traductions.created_at) as day, MONTH(traductions.created_at) as month, YEAR(traductions.created_at) as year, sum(total) as total_day
from traductions
GROUP BY DATE(traductions.created_at),DAYNAME(traductions.created_at), MONTH(traductions.created_at), YEAR(traductions.created_at)
ORDER BY MONTH(traductions.created_at) ASC


