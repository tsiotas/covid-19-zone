# covid-19 zone
Dal 6 Novembre 2020 l'Italia viene divisa in fasce: le regioni assumono un colore a seconda della gravità della situazione legata al diffondersi dell'epidemia di coronavirus.

I file contengono i dati aggiornati delle colorazioni assegnate ogni giorno ad ogni regione.
 
Due file contengono le stesse informazioni storiche in due formati (json e csv)
Esiste un terzo file today.json che contiene la situazione della giornata corrente (aggiornato alle 00:01 di ogni giorno)

# Metodologia di aggiornamento
Gli aggiornamenti vengono inseriti manualmente da fonti governative o testate giornalistiche, il giorno prima in modo da avere le info aggiornate a mezzanotte del giorno successivo 
Alle 00:01 di ogni giorno viene eseguito l'aggiornamento della situazione attuale per il giorno corrente.

Non esiste un aggiornamento attraversi dati open strutturati distribuiti ufficialmente perchè i dati disponibili dal Gverno o dal Ministero della Salute sono rilasciati a volte solo nei giorni feriali e solo nella mattinata durante orari lavorativi.

Il dataset nasce con l'obiettivo di avere uno storico, non tanto di essere affidabile sulla giornata corrente, non ci sono garanzie quindi che quelli del giorno corrente siano esatti, ma abbiamo creato uno script che esegue un parsing ogni minuto su una pagina HTML ufficiale del Governo che ci notifica se esistono dati incongruenti con quelli inseriti, nel caso  in cui la pagina del Governo sia stata aggiornata ad esempio a metà mattinata. In questo modo riusciamo a correggere immediatamente eventuali discrepanze.

# Autori:
Giorgio Tsiotas - Luca Lorello

# Termini di Licenza:
https://creativecommons.org/licenses/by/4.0/deed.it
