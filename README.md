# Stig för iPhone

Personlig GPS-turdagbok med bakgrundsinspelning, topografisk karta, snowboardstatistik och GPX. Kräver iOS 17 eller senare.

## Hämta appen

1. Öppna fliken **Actions** och välj senaste gröna körningen av **Bygg Stig för iPhone**.
2. Hämta artefakten **Stig-iPhone** och packa upp dess ZIP. Installationsfilen heter **Stig.ipa**.
3. Installera SideStore på din iPhone med hjälp av Windows enligt [SideStores guide](https://docs.sidestore.io/docs/installation/install.html).
4. Med Wi-Fi och LocalDevVPN aktiverade: öppna SideStore, välj **My Apps → +** och välj IPA-filen.
5. Starta Stig utomhus, tillåt Exakt plats och prova först en kort tur med låst skärm.

Förnya både SideStore och Stig före sju dagar. Det kan göras på telefonen via Wi-Fi; datorn behövs normalt bara för första installationen. Turer lagras lokalt och flyttas till/från webbappen via GPX.

## Källkod och bygge

Hela projektet finns i **Stig-iPhone-projekt.zip**, inklusive Swift-filer, Xcode-projekt, 17 tester och **INSTALLERA-WINDOWS.md**. Byggflödet packar upp paketet på en standardrunner med macOS, kör testerna och bygger en osignerad IPA för SideStore. Apple-lösenord och certifikat behövs inte hos GitHub. Byggflödet körs bara i publika repo.

Nedför summerar alla nedförsdelar. Fallhöjd är högsta minus lägsta utjämnade höjd. Maxhastighet är högsta GPS-snitt över minst fem sekunder; mätsträckan och en markör visas på kartan.

En grön byggning visar att kompilering och simulatorns tester lyckades. Verklig GPS, låst skärm och batteriförbrukning måste provas på en fysisk iPhone. Svep inte bort Stig från appväxlaren under en tur. Säkerhetskopiera viktiga turer med GPX.
