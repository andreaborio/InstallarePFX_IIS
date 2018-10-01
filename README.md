# Come installare certificato pfx su IIS 

Guida passo su come installare un certificato pfx in IIS 10.


# Importare il certificato pfx 

La prima operazione da fare consiste nell'importare il certificato .pfx in windows server.
Per farlo digitare **mmc** nella finestra run di windows ( windows+r)
![enter image description here](https://image.ibb.co/dX8ADe/mmcura.jpg)
Nella finestra che si apre selezionare File-> Aggiungi/Rimuovi snap-in...
![](https://preview.ibb.co/bT5AeK/mmcconsole.jpg)
  
  Dalla finestra che si apre selezionare Certificati e poi Aggiungi >
  <img src="https://preview.ibb.co/n6ktzK/Cattura.jpg" alt="Cattura" border="0"></a><br />
  Selezionare successivamente "Account del computer" e "Computer locale" nella schermata successiva, cliccare poi "Fine"
 <img src="https://image.ibb.co/khAXte/acca.jpg" alt="acca" border="0"></a>
A questo punto possiamo chiudere la finestra Aggiungi o rimuovi snap-in e ci troveremo una situazione simile
<img src="https://preview.ibb.co/cumu6z/hghgj.jpg" alt="hghgj" border="0">
Ora espandiamo la voce "Certificati" e facciamo clik con il tasto destro su "Personale", selezionando "Tutte le attività"->"Importa"
<img src="https://preview.ibb.co/bCV1KK/xdasc.jpg" alt="xdasc" border="0">

A questo punto si aprirà questa procedura guidata
<img src="https://image.ibb.co/mxV1KK/importazione_Cert.jpg" alt="importazione_Cert" border="0">
Fare **Avanti** -> Selezionare il certificato (cambiare l'estensione nella finestra di selezione file a PFX)
<img src="https://image.ibb.co/cbF1KK/importato.jpg" alt="importato" border="0">
Ora inseriamo la password del certificato **Che abbiamo settato noi se il certificato l'abbiamo generato partendo dalle chiavi diversamente deve esserci fornita dalla società di certificazione**
<img src="https://image.ibb.co/fgN13e/passcert.jpg" alt="passcert" border="0">
Collochiamo il certificato nell'archivio personale e clicchiamo fine.
<img src="https://image.ibb.co/fpGdie/fine.jpg" alt="fine" border="0"></a>

**L'IMPORTAZIONE E' ORA COMPLETA**

## BINDING DEL CERTIFICATO IIS

1. Apriamo IIS
2. Apriamo con il server
3. Selezioniamo il sito su cui vogliamo installare il certificato e clicchiamo su Binding

![](https://www.digicert.com/images/support-images/iis7/iis7-install-4.gif)
Ora su Aggiungi e selezionimo **https** sotto la voce **Tipo**
e dalla lista Certificato SSL selezioniamo quello di nostra proprietà
![](https://www.digicert.com/images/support-images/iis7/iis7-install-6.gif)

Clicchiamo OK
![](https://www.digicert.com/images/support-images/iis7/iis7-install-7.gif)

Riavviamo il sito IIS



# Fine
