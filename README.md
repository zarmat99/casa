# Casa

La pagina con cui guardo la copia digitale di casa mia e ci provo mobili, pareti e pavimenti: https://zarmat99.github.io/casa/

Questo repository contiene solo il codice della pagina (il visore three.js già impacchettato in `visore.min.js`). I dati
della casa stanno in un repository privato: la pagina li legge con l'API di GitHub e un token di sola lettura che resta
nel browser. Per cambiare la casa (l'Editor) serve una password: il token di scrittura sta nel repository privato solo
cifrato con quella password (PBKDF2-SHA256 e AES-GCM, nel browser), e ogni salvataggio è un commit.

Il codice sorgente, i dati e gli strumenti per rifarli stanno sul mio PC; qui arriva solo quello che serve alla pagina.
