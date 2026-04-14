# DC Comics EDA — Data

Place the raw DC Comics dataset here before running the notebook.

## How to get the data

Download **`dc-wikia-data.csv`** from the source repository and save it in this folder:

```
curl -L "https://raw.githubusercontent.com/ghoshpoulami1293/ComicBookUniverse/main/data/dc-wikia-data.csv" \
     -o data/dc-wikia-data.csv
```

Or download it manually from:  
<https://github.com/ghoshpoulami1293/ComicBookUniverse/blob/main/data/dc-wikia-data.csv>

## Column reference

| Column | Description |
|---|---|
| `page_id` | Unique wiki page ID |
| `name` | Character name |
| `urlslug` | Wiki URL slug |
| `ID` | Identity type (Secret, Public, …) |
| `ALIGN` | Moral alignment (Good, Bad, Neutral, …) |
| `EYE` | Eye color |
| `HAIR` | Hair color |
| `SEX` | Gender |
| `GSM` | Gender/Sexual Minority category |
| `ALIVE` | Living or Deceased |
| `APPEARANCES` | Total number of comic appearances |
| `FIRST APPEARANCE` | Month and year of first appearance (string) |
| `YEAR` | Year of first appearance (numeric) |
