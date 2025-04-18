
📦 Linux Terminal Commando's – Basisuitleg

1. `mkdir` – Maak een nieuwe map aan
   **Gebruik**: mkdir mapnaam
   **Voorbeeld**: mkdir projecten
   *Tip*: Gebruik `-p` voor meerdere lagen tegelijk
         mkdir -p projecten/web/portfolio

2. `touch` – Maak een leeg bestand aan
   **Gebruik**: touch bestandsnaam
   **Voorbeeld**: touch notities.txt
   *Tip*: Als het bestand al bestaat, wordt alleen de datum bijgewerkt

3. `mv` – Verplaats of hernoem bestanden/mappen
   **Gebruik**:
     mv oud.txt nieuw.txt         # Hernoemen
     mv bestand.txt ~/Documenten/ # Verplaatsen naar andere map

4. `cp` – Kopieer bestanden of mappen
   **Gebruik**:
     cp bestand.txt kopie.txt     # Bestand kopiëren
     cp -r map1 map2              # Hele map kopiëren (r = recursive)

5. `rm` – Verwijder bestanden of mappen
   **Gebruik**:
     rm bestand.txt               # Verwijder bestand
     rm -r mapnaam                # Verwijder map + inhoud
     rm -ri mapnaam               # Interactieve bevestiging bij verwijderen

6. ls – Toon de inhoud van een map
   Gebruik:
     ls                          # Toon bestanden
     ls -l                       # Toon details (rechten, grootte, datum)
     ls -a                       # Toon verborgen bestanden (zoals .git)
     ls -la                      # Alles + details

7. tree – Toon mapstructuur als boom
   Gebruik:
     tree                        # Boomstructuur van huidige map
     tree ~/Documenten/          # Boomstructuur van een specifieke map
   Tip: Installeer met `sudo dnf install tree` als het niet beschikbaar is

8. cd – Navigeer naar een map
   Gebruik:
     cd mapnaam                  # Ga naar map
     cd ~                        # Ga naar home directory
     cd ..                       # Ga één niveau omhoog
     cd /                        # Ga naar root directory
   Tip: Gebruik `pwd` om je huidige locatie te zien
