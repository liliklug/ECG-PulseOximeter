# Datenformat

## Ziel

Ein einheitliches Datenformat für die Übertragung

der Messwerte zwischen Mikrocontroller und

Visualisierungssoftware.

## Geplante Messwerte

| Messwert | Beschreibung | Einheit |

|----------|--------------|---------|

| Zeitstempel | Zeitpunkt der Messung | ms |

| EKG | EKG-Signal | abhängig vom Sensor |

| Herzfrequenz | Herzschläge pro Minute | BPM |

| SpO2 | Sauerstoffsättigung | % |

## Beispiel

Ein mögliches Datenformat wäre JSON:

{

  "timestamp_ms": 1000,

  "ecg": 512,

  "heart_rate": 72,

  "spo2": 98

}

## Offene Entscheidungen

- Bluetooth Classic oder Bluetooth Low Energy?

- Welche Abtastraten werden benötigt?

- Wie werden fehlende Messwerte behandelt?

- Werden Rohdaten oder berechnete Werte übertragen?

Hinweis: Das dargestellte JSON ist ein vorläufiges Beispiel.

Das tatsächliche Übertragungsformat wird später festgelegt.
