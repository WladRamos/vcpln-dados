# vcpln-dados

Dados públicos usados nos notebooks da disciplina **Visão Computacional e PLN** (curso IASEG), baixados por URL no Google Colab.

Nenhum dado real de ocorrência é publicado aqui: só versões reduzidas de datasets públicos, com a licença original.

## `armas_cftv.zip` (release `armas-cftv-v1`)

Versão reduzida, para fins educacionais, do dataset:

> Ruiz-Santaquiteria, J.; Muñoz, J. D.; Maigler, F. J.; Déniz, O.; Bueno, G. (2023).
> *Action recognition and object detection dataset for firearm-related actions.* Mendeley Data, V2.
> doi:[10.17632/bbzpxhd22j.2](https://doi.org/10.17632/bbzpxhd22j.2)

**Licença: CC BY-NC 3.0**, a mesma da fonte. O uso é não comercial e exige atribuição.

O que foi alterado em relação à fonte:
- quadros amostrados dos vídeos e reduzidos a 640 px no lado maior;
- rótulos convertidos de COCO para o formato YOLO;
- classes renomeadas: Handgun → `pistola`, Machine_Gun → `arma_longa`;
- separação por cena: treino/validação nas cenas P1–P4 e teste na cena P5, que nunca aparece no treino.

Conteúdo: `images/` e `labels/` com `train` (1595), `val` (263) e `teste` (721), além de `videos_teste/` (7 vídeos da cena P5), `data.yaml` e `LEIAME.txt`.

```
wget https://github.com/WladRamos/vcpln-dados/releases/download/armas-cftv-v1/armas_cftv.zip
```
