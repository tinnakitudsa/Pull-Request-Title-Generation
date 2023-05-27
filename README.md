
# Pull-Request-Title-Generation

This project aims to eliminate wasting considerable time thinking about the pull-request name by automated the pull request naming
process. We take four different approaches. 

## Approachs 
- Original BART model “Facebook/bart-base”. [code](https://github.com/tinnakitudsa/Pull-Request-Title-Generation/blob/main/baseline.ipynb)
- Feature extraction + The BART model.
- Feature extraction + The two BART model. [code](https://github.com/tinnakitudsa/Pull-Request-Title-Generation/blob/main/BART2BART.ipynb)
- Feature extraction + The BART model + TextRank algorithm. [code](https://github.com/tinnakitudsa/Pull-Request-Title-Generation/blob/main/bart-with-text-rank.ipynb)

## Dataset
We used [PRTiger dataset](https://github.com/soarsmu/PRTiger).

## Results
| Model  | ROUGE-1 | ROUGE-2 | ROUGE-L |
| ------ | ------ | ------ | ------ |
| BART | 46.8684 | 25.0862  | 42.9303 |
| BART + preprocessing | 46.5925 | 24.7061  | 42.7126 |
| BART + preprocessing + BART | 45.6653 | 23.9111  | 41.6356 |
| BART + preprocessing + TextRank + BART | 46.3706 | 24.5945  | 42.4827 |





## Appendix

- [Final Report](https://github.com/tinnakitudsa/Pull-Request-Title-Generation/blob/main/NLP-final-report.pdf)
- [Final presentation](https://github.com/tinnakitudsa/Pull-Request-Title-Generation/blob/main/NLP_final_present.pdf)
## Authors

- [@NonKhuna](https://github.com/NonKhuna) (BART + preprocessing + TextRank)
- [@tinnakitudsa](https://github.com/tinnakitudsa) (BART base)
- [@sern](https://github.com/sseerrnn) (BART + BART model)
- [@THrapooM](https://github.com/THrapooM) (BART + preprocessing + TextRank)
- [@Alones](https://github.com/pol-alones) (Preprocessing)
- [@Tantawit](https://github.com/Tantawit) (BART model)

