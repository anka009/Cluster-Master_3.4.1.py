# Cluster-Master_3.4.1.py
Cluster-Master 3.4.1 – Streamlit-Testversion

Diese Version ist zum Austesten vor dem lokalen Windows-Port gedacht.

Enthalten:
- Cluster-Master-Hauptanalyse
- Colibri-DBSCAN-Kalibrierung
- gemeinsame Koordinaten-/Kalibrierungslogik
- gemeinsame DBSCAN-Engine
- Colibri kann die aktuell eingestellten eps/min_samples-Werte
  an den Hauptanalysemodus übergeben.

Start:
    pip install -r requirements.txt
    streamlit run cluster_master_3_4_1_streamlit.py

Wichtig:
Diese Version ist zunächst eine Test-/Validierungsversion.
Die Ergebnisse müssen gegen Cluster-Master 3.4 mit bekannten
Testdaten geprüft werden, bevor daraus die finale PC-EXE entsteht.

Methodik:
- DBSCAN-Logik unverändert.
- Default eps im Hauptanalysemodus: 10 µm.
- Default min_samples: 3.
- Voronoi: Mittelwert + 2 SD oder benutzerdefiniertes Maximum.
- Voronoi-Cutoff beeinflusst ausschließlich Voronoi-Kennzahlen.
