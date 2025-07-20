# 📅 Daily Check‑In für Streamer.bot

Dieses Projekt erweitert **Streamer.bot** um ein **Daily Check‑In System**.  
Deine Zuschauer können sich **einmal pro Tag** einchecken und z. B. Punkte, Rollen oder andere Events auslösen.

✅ **!checkin** Befehl im Chat oder über eine Channel‑Point‑Belohnung  
✅ Speicherung über globale Variablen in Streamer.bot  
✅ Einmal pro Tag pro Nutzer  
✅ Fertig vorbereitet als `.sb`‑Export zum einfachen Import

---

## 🚀 Installation (via Import)

### Voraussetzungen
- [Streamer.bot](https://streamer.bot/) ist installiert
- Du hast Moderator‑ oder Adminrechte auf deinem Twitch‑Kanal

---

### 🔧 Import‑Schritte

1. **Streamer.bot starten**  
2. Menü **Tools → Import** öffnen  
3. Auf **Import from File** klicken  
4. Die Datei `daily-checkin.sb` auswählen  
5. Import bestätigen

Nach dem Import findest du eine neue **Action**:
- `Daily Check-in` → Logik für das Einchecken



## 🎯 Channel‑Point‑Belohnung erstellen (Twitch)

Du kannst zusätzlich in Twitch eine **Custom Reward** anlegen, die diese Action auslöst.

1. Gehe in deinen Twitch‑Creator‑Dashboard:  
   **Monetarisierung → Channel Points → Manage Rewards & Challenges**

2. **Neue Belohnung erstellen**:
   - Name: z. B. `Daily Check‑In`
   - Punkte: beliebig (z. B. 1)
   - Beschreibung: „Trage dich täglich ein und sichere dir Vorteile!“

3. **Wichtige Optionen aktivieren**:
   - ✅ **Redemption skips queue** (Einlösungen überspringen die Warteschlange)
   - ✅ **Max 1 per stream** (Belohnung kann nur einmal pro Stream eingelöst werden)
   - ✅ **Max 1 per user per stream** (jeder Nutzer nur einmal pro Stream)

4. **Speichern**.

5. **In Streamer.bot verbinden**:
   - Gehe in **Actions → Daily Check‑In → Triggers**
   - Füge unter **Twitch: Channel Point Reward** deine neue Belohnung hinzu
   - Speichern

Ab sofort kannst du nicht nur mit `!checkin` im Chat einchecken, sondern auch durch die Channel‑Point‑Belohnung.

---

## 🛠️ Anpassen

- Nachrichten ändern: in der Action → Inline Script
- Check‑In‑Liste zurücksetzen: in **Settings → Variables** die `checkin_[name]` leeren

---

**Viel Spaß mit deinem Daily Check‑In System! 🎉**
