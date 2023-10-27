# Como usar seus assets

## Sprites
Quando compilados, as sprites são postas num texture atlas. Portanto, são representadas como arrays.

```csharp
// Using
using Claw;
using Claw.Graphics;

// Carregando atlas
Sprite[] sprites = Assets.Load<Sprite[]>("Sprites/MeuAtlas");

TextureAtlas.AddSprites(sprites);

// Desenhando na tela
Draw.Sprite(TextureAtlas.Sprites["MeuAtlas/MinhaSprite"], Vector2.Zero, Color.White);
```

## Fontes

```csharp
// Using
using Claw;
using Claw.Graphics;

// Definindo campos
private SpriteFont myFont;

// Carregando fonte
myFont = Assets.Load<SpriteFont>("Fontes/MinhaFonte");

// Desenhando na tela
Draw.Text(myFont, "Meu texto...", Vector2.Zero, Color.White);
```

## Mapas

```csharp
// Using
using Claw;
using Claw.Tiled;

// Configurando assets
Tiled.Config = new Config("Jogo.Objetos"); // Prefixo de namespace

Tiled.Config.AddPalettes(("paleta1", TextureAtlas.Sprites["Tilesets/paleta1"])); // Configurando paletas

// Carregando mapa
Tiled.Load(Asset.Load<Map>("Mapas/MeuMapa"));
```

## Áudios

```csharp
// Using
using Claw;
using Claw.Audio;

// Definindo campos
private Music myMusic;
private SoundEffect myEffect;

// Carregando assets
myMusic = Asset.Load<Music>("Audios/Musica"); // Áudio lido por Stream de arquivo
myEffect = Asset.Load<SoundEffect>("Audios/Efeito"); // Áudio carregado na memória

// Dando play em músicas
Game.Instance.Audio.SetMusic(myMusic);

// Dando play em efeitos sonoros
Game.Instance.Audio.Play(myEffect.CreateInstance(SoundEffectGroup.SoundEffect));
```