- Il logo Holland & Sherry non compariva: la pulizia degli SVG tagliava il DOCTYPE a meta' quando aveva un subset interno fra parentesi quadre, lasciando un `]>` orfano che rendeva il file non valido. Il browser lo scartava in silenzio. File riparato, regex corretta in `tools/normalize-brand-logos.py`, e `tools/gen-suppliers.py` ora rifiuta di pubblicare un SVG che non sia XML valido.

