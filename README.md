# Eigene Sprachmodelle feintunen und nutzen

Repository zum Workshop.

Folgende Basispakete sollten installiert sein:

* `numpy`
* `pandas`
* `tqdm`
* `sklearn`
* `matplotlib`
* `seaborn`

Für die Vorverarbeitung brauchen wir `spacy`.

Das Finden von Informationen geschieht mit:

* `torch`
* `transformers`
* `sentence_transformers`

Für die Inferenz der generativen Modelle wird folgendes benötigt:
* `gptqmodel`
* `exllamav2`

Für das Training eigener generativer Modelle:
* `trl`
* `unsloth`
* `liger_kernel`
* `peft`
* `datasets`

Alternativ gern `requirements.txt` oder `pyproject.toml` verwenden.
Wenn sich nicht alles installieren lässt, klären wir das direkt im
Workshop. 

Es läuft auch unter Windows, allerdings ist die Installation etwas
*hakelig*. Eine Variante, wie es bei mir funktioniert hat, findet
ihr unter [WINDOWS.md](WINDOWS.md).
