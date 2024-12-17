# Team-A
Oppgave
Oppgave 1: Opprett en Azure Storage-konto med Private Endpoint og Key Vault
Mål
Utforske hvordan du kan sikre Azure Storage med en Private Endpoint og håndtere hemmeligheter med Azure Key Vault.

Forutsetninger
Du trenger en Azure Subscription.
Bicep og Azure CLI må være installert.
Oppgavebeskrivelse
Lag en Bicep-fil som heter secure-storage.bicep. Filen skal opprette følgende ressurser:

Ressursgruppe: For å holde alt i én gruppe.
Azure Storage-konto: Bruk Standard_LRS som SKU.
Virtual Network (VNet): Opprett et nettverk med minst to subnets.
Private Endpoint: Koble Storage-kontoen til det private nettverket.
Azure Key Vault: For å lagre tilgangsnøkkelen til Storage-kontoen som en hemmelighet.
Krav
Storage-kontoens tilgang skal kun tillates via Private Endpoint (ikke offentlig tilgang).
Key Vault skal ha en hemmelighet som lagrer nøkkelen til Storage-kontoen.
Bruk parameterisering for å gjøre løsningen gjenbrukbar (f.eks. navn, plassering, SKU).
Leveranse
En komplett Bicep-fil som oppretter alle ressursene.
Verifiser at Private Endpoint er konfigurert, og at nøkkelen til Storage-kontoen er lagret i Key Vault.
