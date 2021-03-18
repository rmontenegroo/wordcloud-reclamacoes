## Projeto final de BI

> Cria uma wordcloud a partir de dados obtidos da base src/db/base_reclamacoes.csv
> É possível criar a wordcloud usando o conteúdo dos atributos ou decompor esse conteúdo
> completamente em tokens (modo default)

```
usage: reclamacoes [-h] [--target {empresa,servico,estado,area}] [-r] [-v] [-o OUTPUT_FILE] [-m MASK_FILE]

Análise de reclamações de empresas por WordCloud

optional arguments:
  -h, --help            show this help message and exit
  --target {empresa,servico,estado,area}
                        Atributo de análise. (Default: 'empresa')
  -r, --raw-mode        Processa os registros mas não tokeniza. (Default: False)
  -v, --verbose         Executa em modo verbose. (Default: False)
  -o OUTPUT_FILE, --output-file OUTPUT_FILE
                        Arquivo de saída. (Default: 'wordcloud_[TARGET].png')
  -m MASK_FILE, --mask-file MASK_FILE
                        Arquivo de imagem para utilizar como máscara. (Default: 'img/brazil_mask.png' (mais de 40 tokens) ou 'img/full_mask.png' (menos de 40 tokens))
```