# Privacy Policy — TrustCheck

Last updated: 2026-07-10

## English

**Summary:** TrustCheck runs fully offline. The extension collects no personal data, has no user account, no tracking and no server of its own, and sends no data anywhere. All checks happen exclusively and locally in your browser.

**What data is processed and where:**

1. Page content, locally: To count contact info and social links, the extension reads the visible text and links of the current page. This evaluation happens fully locally in your browser. The page content is neither stored nor transmitted.
2. Address (URL), locally: The address of the page is checked locally for fraud patterns. This too never leaves your device.
3. Local storage: Results, settings and two local counters (pages checked / risks detected, for the popup display) are stored on your device via `chrome.storage.local` (results are cached for 24 hours). This data never leaves your device and is never shared with us.

**No network access takes place.** The extension contains no outbound request whatsoever (no `fetch`, no XHR), verifiable by scanning all loaded modules.

**What does NOT happen:** No collection of personal data, no transmission of data to the outside, no sale or sharing of data, no advertising or analytics trackers, no transmission of passwords, form content or payment data, no server of ours.

**Permissions and why:**

- `storage`: only for the local 24 hour cache, the settings and the two local counters.
- Content script on all pages (`matches: <all_urls>`): required because the trust score is meant to be computed on any page. Without broad access, the extension could only warn on a whitelist of pages, which would undermine its purpose (warning precisely on unknown pages). Because there is no network call, the extension needs no `host_permissions` and no `activeTab`.

**Contact:** Sadu Pamdir — via the [GitHub repository](https://github.com/sadu-pamdir/trustcheck).

---

## Deutsch

**Kurzfassung:** TrustCheck läuft vollständig offline. Die Erweiterung sammelt keine personenbezogenen Daten, hat kein Nutzerkonto, kein Tracking und keinen eigenen Server, und sendet überhaupt keine Daten nach aussen. Die gesamte Prüfung passiert ausschliesslich und lokal in deinem Browser.

**Welche Daten verarbeitet werden und wo:**

1. Seiteninhalt lokal: Um Kontakt-Infos und Social-Links zu zählen, liest die Erweiterung den sichtbaren Text und die Links der aktuellen Seite. Diese Auswertung passiert vollständig lokal im Browser. Der Seiteninhalt wird nicht gespeichert und nicht übertragen.
2. Adresse (URL) lokal: Die Adresse der Seite wird lokal auf Betrugsmuster geprüft. Auch das verlässt das Gerät nicht.
3. Lokaler Zwischenspeicher: Ergebnisse, Einstellungen und zwei lokale Zähler (geprüfte Seiten / erkannte Risiken für die Popup-Anzeige) werden über `chrome.storage.local` auf dem Gerät gespeichert (Ergebnis-Cache für 24 Stunden). Diese Daten verlassen das Gerät nicht und werden nicht mit dem Anbieter geteilt.

**Es findet kein Netzwerkzugriff statt.** Die Erweiterung enthält keinen einzigen ausgehenden Request (kein `fetch`, kein XHR), überprüfbar per Scan über alle geladenen Module.

**Was NICHT passiert:** Keine Erfassung personenbezogener Daten, keine Datenübermittlung nach aussen, kein Verkauf oder Weitergabe von Daten, keine Werbe- oder Analyse-Tracker, keine Übermittlung von Passwörtern, Formularinhalten oder Zahlungsdaten, kein Anbieter-Server.

**Berechtigungen und warum:**

- `storage`: nur für den lokalen 24-Stunden-Cache, die Einstellungen und die zwei lokalen Zähler.
- Content-Script auf allen Seiten (`matches: <all_urls>`): nötig, weil der Vertrauens-Score auf jeder beliebigen Seite berechnet werden soll. Ohne breiten Zugriff könnte die Erweiterung nur auf einer Whitelist von Seiten warnen, was den Zweck (Warnung genau auf unbekannten Seiten) untergraben würde. Da kein Netz-Call stattfindet, braucht die Erweiterung kein `host_permissions` und kein `activeTab`.

**Kontakt:** Sadu Pamdir — über das [GitHub-Repository](https://github.com/sadu-pamdir/trustcheck).
