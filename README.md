# Eigene Sprachmodelle feintunen und nutzen

Repository zum Workshop.

## Pakete
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
* `tantivy`
* `usearch`

Für die Inferenz und das Training der generativen Modelle wird folgendes benötigt:
* `trl`
* `unsloth`
* `liger_kernel`
* `peft`
* `datasets`
* `bitsandbytes`
* `einops`
* `openai`

Alternativ gern `pyproject.toml` verwenden. Für `unsloth` und `vllm`
wird `unsloth.toml` benötigt, `sglang` benötigt leider aktuell eine
eigene Umgebung, weil das Gemma-Modell in der neuesten Version von `sglang`
nicht funktioniert.
Wenn sich nicht alles installieren lässt, klären wir das direkt im
Workshop. 

Es läuft auch unter Windows, allerdings ist die Installation etwas
*hakelig*. Gleiches gilt für AMD-Grafikkarten, das kann ich ohne
entsprechende Karte leider nicht testen.

Wir arbeiten mit unterschiedlichen Sprachmodellen. Je nach Internet-Verbindung
kann es sinnvoll sein, diese vorher herunterzuladen:

## Modelle
Für die Einleitung verwenden wir:
* google-bert/bert-base-multilingual-cased
* nlptown/bert-base-multilingual-uncased-sentiment
* MoritzLaurer/mDeBERTa-v3-base-mnli-xnli

Feintuning von BERT verwendet:
* dbmdz/bert-base-german-uncased

Für Embeddings nutzen wir diese Modelle:
* multi-qa-MiniLM-L6-cos-v1
* google/embeddinggemma-2
* microsoft/harrier-oss-v1-0.6b

Wir benutzen folgende Cross-Encoder:
* cross-encoder/ms-marco-MiniLM-L-6-v2
* mixedbread-ai/mxbai-rerank-large-v1
* Qwen/Qwen3-Reranker-0.6B

Bei der generativen Inferenz arbeiten wir mit diesen Modellen:
* Qwen/Qwen3.5-9B
* google/gemma-4-12B-it
* google/gemma-4-12B-it-qat-w4a16-ct
* google/gemma-4-12B-it-assistant
* turboderp/Qwen3.8-27B-exl3 
* GestaltLabs/Qwen3.8-27B-DFlash-EXL3-4bit
* ISTA-DASLab/Qwen3.8-27B-GSQ-RCO-GGUF:IQ3_S-mtp

Für das generative Finetuning werden folgende Modelle benötigt:
* Qwen/Qwen3-0.6B
* meta-llama/Llama-3.2-1B-Instruct
* HuggingFaceTB/SmolLM2-1.7B-Instruct
* microsoft/Phi-3.5-mini-instruct

Datasets:
* sentence-transformers/all-nli
