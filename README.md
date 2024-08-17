Groep 4 - Jelle, Ilias, Sem, Mayk, Robbe, Jentse, Cedric
# Email PKI Evolution
In deze opdracht stellen we ons tot doel om een configuratie op te zetten waarmee we e-mails kunnen voorzien van digitale handtekeningen en encryptie. Het proces omvat verschillende stappen, waaronder het genereren en toepassen van digitale handtekeningen om de authenticiteit van de verzender te waarborgen en het implementeren van encryptie om de vertrouwelijkheid van de inhoud te waarborgen. Door deze maatregelen toe te passen, streven we ernaar om de veiligheid en integriteit van onze communicatie via e-mail te verbeteren.

## Samenvatting van de opdracht
Voor deze opdracht moeten wij gebruikmaken van digitale handtekeningen op een Linux-systeem. Hiervoor hebben wij gekozen voor Evolution als mailclient. Met Evolution zullen wij een versleutelde en ondertekende e-mail versturen door gebruik te maken van S/MIME. De digitale handtekening maakt gebruik van een hashfunctie waarmee de integriteit van het bericht wordt verzekerd, en voor de versleuteling wordt gebruikgemaakt van asymmetrische encryptie.
Om de integriteit van de publieke sleutel van de afzender te waarborgen, wordt er gebruikgemaakt van een PKI-systeem, namelijk EJBCA. Binnen EJBCA moet een certificaat worden gegenereerd voor het e-mailaccount. De opties voor Data Encryption en Digital Signing moeten worden ingeschakeld in EJBCA. Het certificaat moet worden gedownload vanuit EJBCA en geïmporteerd worden in Evolution. In de eerste opdracht komt het certificaat van de eigen lokale PKI EJBCA, wat betekent dat zowel de zender als de ontvanger binnen de lokale PKI-infrastructuur worden gevalideerd.
Bij de tweede opdracht wordt gebruikgemaakt van een officieel certificaat van Actalis. Dit certificaat wordt in Evolution geïmporteerd en biedt de mogelijkheid om e-mails te ondertekenen en te versleutelen met een certificaat dat door een erkende externe CA is uitgegeven.

## Verslagen / Documentaties
- [Email signing with Actalis](./verslagen/mail_signing_actalis.md)
- [Email signing & encrypting with EJBCA](./verslagen/EJBCA_Email_encryption_and_signing.md)
