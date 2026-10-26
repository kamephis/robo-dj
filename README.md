# Robo DJ

Ein niedlicher 3D-Roboter, der in den Pausen einer Präsentation hinter einem DJ-Pult mit zwei Plattenspielern auflegt, tanzt und eine Lichtshow zeigt.

## Starten

`index.html` im Browser öffnen. Es gibt keinen Build-Schritt und keine Abhängigkeiten zum Installieren. three.js (0.149.0) und die Schriften werden per CDN geladen, deshalb braucht es eine Internetverbindung.

Auf GitHub Pages veröffentlichen: *Settings → Pages → Deploy from a branch → `main` / root*.

## Funktionen

- **Musik**: wird live im Browser mit der Web Audio API erzeugt. Stile: House, Retro-Disco, Lo-Fi. Regler für Tempo, Lautstärke und DJ-Filter.
- **Tanz**: Auto, Auflegen, Hände hoch, Robot Dance, Headbang, Pirouette, Winken.
- **Licht & Effekte**: Lichtshow, LED-Wand (folgt dem Spektrum), Laser, Discokugel, Nebel, Stroboskop (bei „Bewegung reduzieren“ deaktiviert).
- **FX-Pad**: Konfetti, Air-Horn, Scratch, Drop.
- **Pausen-Timer**: Banner-Text, 5–30 Minuten Countdown. Am Ende winkt der Roboter und die Musik wird ausgeblendet.
- Roboter anklicken = Boop.

## Tastatur

| Taste | Aktion |
|---|---|
| Leertaste | Musik an/aus |
| 1–7 | Tanz wählen |
| S / W / L / D / N / B | Lichtshow / LED-Wand / Laser / Discokugel / Nebel / Stroboskop |
| K / A / X / R | Konfetti / Air-Horn / Scratch / Drop |
| F | Vollbild |
| H | Steuerung aus-/einblenden |

Musik startet erst nach einem Klick, weil Browser Autoplay mit Ton blockieren.
