# Verslag: Implementatie S/MIME

### Inleiding:
We zullen onze certificaten aanvragen bij Actalis, aangezien het een van de weinige CAs is die een gratis S/MIME-certificaat aanbiedt. Het heeft ook als voordeel dat de ontvangers van onze email geen root CA moeten downloaden op hun machine.

### 1. Account aanmaken
1. Ga op actalis.com en maak een account aan.  

![Image of actalis login](../resources/afbeeldingen/signup.png)

2. Vul jouw gegevens in.
   
![Image of actalis registration](../resources/afbeeldingen/registration.png)

3. Bij de laatste stap krijg je het wachtwoord van je certificaat te zien. Bewaar dit goed, aangezien dit de laatste keer is dat je het wachtwoord zult zien.

### 2. Certificaat
1. In je mailbox zou je normaal gesproken een certificaat als bijlage moeten hebben ontvangen.
![Image of received certificates](../resources/afbeeldingen/received_certificate.png)

2. Download het certificaat, zodat we het later kunnen importeren in onze Evolution-mailclient. We zullen dat certificaat gebruiken om e-mails te ondertekenen.

### 3. Certificaat importeren in Evolution
1. Open Evolution
2. Ga naar edit --> preferences
![Image of evolution settings](../resources/afbeeldingen/evolution_preferences.png

3. Klik op “certificates” en nadien op “import”.
![Image of certificate import](../resources/afbeeldingen/evolution_certificate_import.png)
4. Selecteer het certificaat die je net hebt opgeslagen.
5. Voer het wachtwoord in dat je bij het aanvragen van het certificaat te zien kreeg.

### 4. Certificaat linken aan e-mail account
1. Open Evolution
2. Ga naar edit --> preferences
![Image of evolution settings](../resources/afbeeldingen/evolution_preferences.png

3. Selecteer jouw email account en klik op “edit”
![Image of mail account](../resources/afbeeldingen/evolution_edit_mailaccountpng.png)
4. Klik vervolgens op “security”. Bij “signing certificate” klik op “select”.
![Image of selected cert](../resources/afbeeldingen/evolution_select_certificate.png)
5. Selecteer de juiste certificaat en klik op “ok”.

### 5. Getekende mail verzenden
1. Maak een mail op die je naar een persoon wilt verzenden.
2. Klik op “options” en vervolgens op “S/MIME sign”
![Image of signing mail](../resources/afbeeldingen/evolution_sign_email.png)

### 6. Resultaat
Zoals je kunt zien, krijgt de ontvanger (afhankelijk van de mail-client) een medaille te zien bij jouw e-mail. Dit betekent dat de e-mail is ondertekend en dat je er zeker van kunt zijn dat de ontvanger is wie hij zegt te zijn.
![Image of proof mail](../resources/afbeeldingen/email_result.png)
