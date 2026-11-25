# Casa

La pagina con cui guardo la copia digitale di casa mia e ci provo mobili, pareti e pavimenti: https://zarmat99.github.io/casa/

Questo repository contiene solo il codice della pagina (il visore three.js già impacchettato in `visore.min.js`). I dati
della casa stanno in un repository privato: la pagina li legge con l'API di GitHub e un token di sola lettura, e ogni
salvataggio dell'Editor è un commit fatto con un token di scrittura. I token sono salvati solo cifrati con due password
(PBKDF2-SHA256 da 600 000 giri e AES-GCM, nel browser): quello di lettura in `chiave.json`, qui accanto, con la
password per guardare; quello di scrittura nel repository privato, con la password dell'Editor. Le password non sono
scritte da nessuna parte.

Il codice sorgente, i dati e gli strumenti per rifarli stanno sul mio PC; qui arriva solo quello che serve alla pagina.
