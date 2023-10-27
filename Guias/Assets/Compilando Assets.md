# Como usar o Clawssets
Baixe o último **release**. A pasta "Clawssets" terá o executável, as dependências e um arquivo batch. Para facilitar o uso do compilador, altere o seu **PATH**, inserindo o diretório do Clawssets.

```
> setx /M PATH "%PATH%;C:\Local\Do Meu\Clawssets"
```

Já para compilar os assets, basta utilizar o comando "Clawssets" em uma dessas formas:

```
> Clawssets [config].cb
> Clawssets
```

Caso não digite o nome do arquivo de configuração, o compilador irá procurar um arquivo **.cb** na pasta. Se não encontrar, ele pedirá que você especifique o caminho inteiro.

# Configurando a compilação
A compilação dos assets se baseia num arquivo **.cb**, que indica os assets que serão compilados e para onde serão. <br />
A estrutura desse arquivo é:

```
| Output (Relativo ao arquivo)
../../../Game.Windows/bin/Debug/Assets
../../../Game.Windows/bin/Release/Assets

| [Tipo de Asset]:[Nome do Grupo]
#Texture:Meu Atlas
sprite.png

#SpriteFont:Fontes/Hud
font.csf
```

As primeiras linhas representam o local para onde os assets serão copiados após a compilação. Já o "#" indica um grupo de assets. <br />
Toda linha que inicia com "|" é ignorada. <br />
Os tipos de grupos são:

## Texture
Representa um grupo de images (.png, .jpg, .bmp) e são compilados num único arquivo, em que o nome das sprites é registrado como `[Nome do grupo]/[Nome da sprite (sem extensão)]`. <br />
Um atlas não pode ultrapassar o tamanho de 2048x2048 (nem todo o espaço será bem aproveitado).

## SpriteFont
Se baseiam num arquivo JSON **.csf** e servem para compilar fontes instaladas na sua máquina (ao invés de baseadas numa imagem). <br />
A estrutura do arquivo é:

```jsonc
{
    "FontName": "Arial", // Nome da fonte
    "Size": 12, // Tamanho da fonte
    "Spacing": 0, // Espaçamento horizontal entre caracteres (float)
    "Style": "Regular", // Estilo da fonte

    "CharacterRegions": [ // Regiões de caracteres que serão inclusos
        { "Start": 32, "End": 126 }, // ' ', '!', '"'...
        { "Start": 127, "End": 252 }
    ]
}
```

## Audio
Se baseiam em arquivos de áudio **.wav** (PCM). <br />
Para garantir que a compilação seja bem sucedida, os arquivos precisam ser Mono/Stereo e terem **até** 48kHz (áudios com menos que isso serão re-sampleados).

## Map
Os objetos devem ter o tipo como o namespace (sem o prefixo), do que você quer instanciar.<br />
Os assets do tipo `Map` são baseados nas exportações JSON do Tiled. Para que isso funcione, você deve marcar as seguintes opções de importação: <br />
![TiledPreferences](/Imagens/TiledExport.png)