# CLI

Faça download do pacote do MeasureSoftGram no PyPi através do comando:
```bash
pip install msgram
```

Após a instalação do pacote execute o comando abaixo para verificar se o msgram foi instalado.
```bash
msgram --help
```

Caso os seguintes textos forem exibidos na tela, significa que o measure foi instalado com sucesso na sua máquina e está pronto para uso.
```bash
usage: msgram [-h] {init,list,extract,calculate,norm_diff,diff} ...

Command line interface for measuresoftgram

options:
  -h, --help            show this help message and exit

subcommands:
  {init,list,extract,calculate,norm_diff,diff}
                        sub-command help
    init                Create a init file `.measuresoftgram` with your default organization, product and repositories
    list                Listing configurations parameters.
    extract             Extract supported metrics
    calculate           Calculates all entities
    norm_diff           Calculate the norm difference between the planned metrics and the developed.
    diff                Calculates differences between planned and developed values. Returns the result vector.

Thanks for using msgram!
```
