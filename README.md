[![GloBI Review by Elton](../../actions/workflows/review.yml/badge.svg)](../../actions/workflows/review.yml) [![GloBI](https://api.globalbioticinteractions.org/interaction.svg?accordingTo=globi:globalbioticinteractions/trophiCH&refutes=true&refutes=false)](https://globalbioticinteractions.org/?accordingTo=globi:globalbioticinteractions/trophiCH)

Configuration to help Global Biotic Interactions (GloBI, https://globalbioticinteractions.org) index: 

Reji Chacko, M., Albouy, C., Altermatt, F., Brändle, M., Casanelles Abella, J., Boussange, V., Campell, F., Ellis, W. N., Fopp, F., Gossner, M. M., Ho., H., Joss, A., Kipf, P., Neff, F., Petrović, A., Prié, V., Tomanović, Ž., Zimmerli, N., Pellissier, L. (2024). trophiCH v1 - a food web for Switzerland. EnviDat. https://www.doi.org/10.16904/envidat.467.

See also 

Reji Chacko, M., Albouy, C., Altermatt, F. et al. A species-level multi-trophic metaweb for Switzerland. Sci Data 12, 1164 (2025). https://doi.org/10.1038/s41597-025-05487-7

## Provenance

To help facilitate data access, the data archive at ```https://www.envidat.ch/dataset/4f9547a1-3018-46f1-a399-09d65a3223f3/resource/6d7f57cc-a98f-4513-9c65-c0230a15bba7/download/trophich.zip``` was captured/tracked using

```
preston track https://www.envidat.ch/dataset/4f9547a1-3018-46f1-a399-09d65a3223f3/resource/6d7f57cc-a98f-4513-9c65-c0230a15bba7/download/trophich.zip
```

which ended with

```
<https://www.envidat.ch/dataset/4f9547a1-3018-46f1-a399-09d65a3223f3/resource/6d7f57cc-a98f-4513-9c65-c0230a15bba7/download/trophich.zip> <http://purl.org/pav/hasVersion> <hash://sha256/35bb5dabfa41666fd814abd9d2b24b474f32f453dc7a174faefcd8bb32331c19> <urn:uuid:6d7761e8-5e7c-4de0-853b-c2acdf9ba674> .
``` 

as reproduced by 

```
preston cat\
 --remote https://softwareheritage.org,https://linker.bio\
 hash://sha256/527044fe37cd404d077e83574a3a8a78209af68ce71f15f55f0e911b4cf86854as\
 | tail -n1
```

Following, ```03_references.tsv``` was generated using

```
preston cat\ 
 --remote https://softwareheritage.org,https://linker.bio\
 'zip:hash://sha256/35bb5dabfa41666fd814abd9d2b24b474f32f453dc7a174faefcd8bb32331c19!/trophiCH/data/03_references.xlsx'\
 > 03_references.xlsx
```

and, ```01_final_metaweb.tsv.gz``` was generated using

```
preston cat\ 
 --remote https://softwareheritage.org,https://linker.bio\
 'zip:hash://sha256/35bb5dabfa41666fd814abd9d2b24b474f32f453dc7a174faefcd8bb32331c19!/trophiCH/data/01_final_metaweb.csv'\
 | mlr --icsv --otsvlite cat\
 | gzip\
 > 01_final_metaweb.tsv.gz
```
