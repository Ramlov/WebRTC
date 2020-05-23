# WebRTC til brug på en FiveM server med GCPhone

## Opsætning af WebRTC
* Step 1 Download alle filerne fra min github https://github.com/Ramlov/WebRTC
* Step 2 Åben port 3478
* Step 3 åben filen der hedder turn og ændre de ting der står deri. (Der hvor der står cd C:\Users\admin\Desktop\turn, denne skal du ændre til at passe med din computer og hvor du har placeret den i. Dette kan findes i stifinder)
* Step 4 Kopier alle tingene fra turn.txt
* Step 5 Åben Windows PowerShell
* Step 6 Indsæt det du lige har kopieret. (Brug CTRL+V)
* Step 7 Tryk enter.

Nu kører din WebRTC

## Opsætning af GCPhone
* Step 1 Gå ind i din GCPhone - HTML - static - config - config.json
* Step 2 Find linjen hvor der står ```"useWebRTCVocal": true,```
* Step 3 Sørg for at der står true
* Step 4 Indsæt alle dine væredier, så det ligner dette
```  "useWebRTCVocal": true,
  "RTCConfig": {
    "iceServers": [{
      "urls": ["turn:127.0.0.1:3478"],
      "username": "ændrebruger",
      "credential": "ændrekode"
    }]
  },```
 
