# Installation unter Windows

## UV
Die Installation klappt am besten mit `uv`. Dessen Installation ist hier gut beschrieben: https://docs.astral.sh/uv/getting-started/installation/

## Erzeugung eines neuen Projekts

Neues Python-Environment mit Python 3.12 erzeugen und aktivieren. Dazu ein Verzeichnis anlegen, dorthin wechseln, `uv init` aufrufen. Mit `uv python list` die möglichen Python-Versionen anschauen und 3.12 mit `uv python install` installieren. 3.13 geht leider nicht, weil manche Pakete nur für 3.12 als Wheels vorliegen.

## Visual Studio installieren

Wird gebraucht, da C-Compilter nötig ist.

## Cuda-Toolkit installieren

https://developer.nvidia.com/cuda-downloads?target_os=Windows&target_arch=x86_64&target_version=11&target_type=exe_local

## Pytorch mit Cuda installieren
uv pip install torch --index-url https://download.pytorch.org/whl/cu126

## Notwendige Pakete herunterladen und installieren

* Triton von https://github.com/woct0rdho/triton-windows/releases/download/v3.2.0-windows.post10/triton-3.2.0-cp312-cp312-win_amd64.whl
* Flash Attention von https://huggingface.co/lldacing/flash-attention-windows-wheel/resolve/main/flash_attn-2.7.4%2Bcu126torch2.6.0cxx11abiFALSE-cp312-cp312-win_amd64.whl

Direkt im aktivierten Environment mit `pip` installieren

# Jetzt den Rest mit `pip` oder `uv add` installieren
