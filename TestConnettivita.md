Di seguito una serie di test che dimostrano il corretto funzionamento della rete, la raggiungibilità tra VLAN, la DMZ e i servizi principali.

### 1. Ping tra PC della stessa VLAN
<div style="display: flex; align-items: center; gap: 20px;">
<div style="flex: 1;">
Verifica che i dispositivi appartenenti alla stessa VLAN possano comunicare correttamente.
Questo test conferma il corretto funzionamento dello switching L2 e dell’assegnazione delle VLAN.
</div>
<img src=" img/gifNet/pcStessaVlan.gif" width="350">
</div>

---

### 2. Ping tra PC di VLAN diverse
<div style="display: flex; align-items: center; gap: 20px;">
<div style="flex: 1;">
Test che dimostra il funzionamento del routing inter‑VLAN.
I pacchetti vengono instradati dallo switch L3 verso la VLAN di destinazione.
</div>
<img src=" img/gifNet/pcDiversaVlan.gif" width="350">
</div>

---

### 3. Ping verso il Server nella DMZ
<div style="display: flex; align-items: center; gap: 20px;">
<div style="flex: 1;">
Verifica che i client interni possano raggiungere il server nella DMZ.
Questo test dimostra il corretto funzionamento dell’ASA.
</div>
<img src=" img/gifNet/PingServerDMZ.gif" width="350">
</div>

---

### 4. Ping dal Server DMZ verso l’interno
<div style="display: flex; align-items: center; gap: 20px;">
<div style="flex: 1;">
Test mostra che il traffico in uscita dalla DMZ verso la rete interna viene correttamente bloccato dall'asa che permette al server nella DMZ di rispondere a ping o richieste di servizi ma blocca qualsiasi tentativo di comunicazione verso l'interno iniziato dal server stesso
</div>
<img src=" img/gifNet/PingDelServerDMZ.gif" width="350">
</div>

---

### 5. Accesso al sito web della scuola (DMZ)
<div style="display: flex; align-items: center; gap: 20px;">
<div style="flex: 1;">
Dimostrazione dell’accesso HTTP al sito ospitato nella DMZ da parte di un PC esterno alla rete della scuola,
dimostra il corretto funzionamento di NAT statico e acl che permettono protocollo HTTP
</div>
<img src=" img/gifNet/SitoScuola.png" width="350">
</div>

---

### 6. Configurazione Server Mail

<div style="display: flex; align-items: center; gap: 20px;">
<div style="flex: 1;">
Server Mail nella DMZ
</div>
<img src=" img/gifNet/MailServer.png" width="700">
</div>

<br><br>

<div style="display: flex; align-items: center; gap: 20px;">
<div style="flex: 1;">
Host Mail nella rete della scuola
</div>
<img src=" img/gifNet/MailConfig.png" width="700">
</div>

<br><br>

<div style="display: flex; align-items: center; gap: 20px;">
<div style="flex: 1;">
Server DNS nella LAN amministrazione
</div>
<img src=" img/gifNet/MailDNS.png" width="700">
</div>

---


### 7. Test del Mail Server
<div style="display: flex; align-items: center; gap: 20px;">
<div style="flex: 1;">
Verifica del funzionamento del server di posta nella DMZ:
invio, ricezione e comunicazione con la rete interna tramite SMTP/POP3/IMAP.
</div>
<img src=" img/gifNet/Mail.png" width="700">
</div>

---
