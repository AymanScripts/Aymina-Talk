# Aymina-Talk

Lokale OmeTV-achtige MVP met React/Vite, Express, Socket.IO en WebRTC.

## Starten

```bash
npm install
npm run dev
```

Open twee browservensters op `http://localhost:5173`, geef beide toestemming voor camera en microfoon en klik in beide vensters op **Start talking**. De backend draait op poort 3001.

`npm run build` bouwt de frontend; `npm run start` serveert de build en start de signalingserver. `npm run lint` controleert TypeScript.

## Bekende beperkingen

De lokale MVP gebruikt een publieke Google STUN-server. STUN is niet voldoende voor elke netwerkcombinatie; voeg voor betrouwbare productieverbindingen een configureerbare TURN-server toe. Rapporten worden momenteel alleen als lokale sessie-event geregistreerd en er worden geen audio-, video- of persoonsgegevens opgeslagen.
