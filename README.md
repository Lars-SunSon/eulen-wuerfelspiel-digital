# Eulen-Würfelspiel digital (inoffiziell)

Eine einzige `index.html`, läuft offline im Browser (Handy, Tablet, PC). Erweiterung des digitalen Wertungsblocks
`eulen-wuerfelspiel`: Würfel, Karten und Spielblock lassen sich komplett in der App spielen.

**Beim Start der Partie wählst du:**
- ein Spieler oder mehrere Spieler (2 bis 6) an einem Gerät
- Würfel in der App oder echte Würfel
- Karten in der App oder echte Karten

**Würfel:** zwei W12, auf der 1 sitzt die Eule. Es zählt der höhere Würfel, die Eule gilt als 1.
- Eule und eine Zahl, die schon in der Zeile steht: Die Eule rettet, nichts wird eingetragen, du wirfst nochmal.
- Eule und neue Zahl: Die Zahl wird normal eingetragen.
- Zwei Eulen: Pasch.
- Doppelte Zahl ohne Eule: genullt, außer ein Wiederholungs-Joker wurde vorher angesagt.

**Pasch und Karten:** Bei einem Pasch zieht die App drei Karten, eine davon wird gewählt. Das Deck (30 Karten) ist ein
**eigenes Deck dieser App** und enthält keine Karten aus dem Originalspiel. Karten, die einen neuen Wurf verlangen,
würfeln direkt in der App.

**Annahmen, die nicht aus dem Spiel bestätigt sind** (Konstanten oben in `index.html`, leicht änderbar):
- Auch zweimal dieselbe Zahl gilt als Pasch.
- Jeder Pasch (auch der Pasch-Joker) zieht `PASCHKARTEN = 3` Karten.
- Zusammensetzung und Wirkung des Decks (`KARTEN`, `DECK`) sind frei erfunden.

**Mehrere Spieler:** Oben tippst du einen Spieler an. „Nächster Spieler“ springt zum nächsten, der noch spielt. Sind alle
fertig, geht es für alle in die nächste Runde. Ab 222 Punkten wird die Runde für alle zu Ende gespielt, am Ende gibt es eine
Rangliste (bei Gleichstand gewinnt, wer seltener genullt hat).

Der Spielstand bleibt im Browser des Geräts gespeichert (`localStorage`, eigene Schlüssel `hdp2_*`). Rückgängig (↶) nimmt
die letzte Eingabe zurück.

**Hinweis:** Inoffizielles Fan-Hilfsmittel, nicht vom Verlag des Spiels und nicht mit ihm verbunden. Alle Namen und
Spielinhalte gehören ihren Inhabern. Es enthält keine Grafiken, Karten oder Texte aus dem Spiel.

Schrift: Poppins (SIL Open Font License 1.1, Indian Type Foundry), eingebettet. Keine externen Dienste, kein Tracking.
