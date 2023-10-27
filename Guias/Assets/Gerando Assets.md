# Como gerar assets por código

## Imagens
### Gerando manualmente
```csharp
// Using
using Claw;
using Claw.Graphics;

// Gerando
int width = 3, height = 3;
Texture texture = new Texture(width, height,
    Color.White, Color.White, Color.White, // Color
    0xff000000, 0xff000000, 0xff000000, // HEX
    new Color(1f, 1f, 1f, 1f), Color.Red, new Color(255, 255, 255) 
);

// Transformando em sprite (Opcional)
Sprite sprite = new Sprite(texture, "Nova Sprite", new Rectangle(0, 0, 3, 3));

TextureAtlas.AddSprite(sprite);
```

### Gerando com surface
```csharp
// Using
using Claw;
using Claw.Graphics;

// Definindo campos
private RenderTarget surface;

// Inicializando
surface = new RenderTarget(64, 64);

// Desenhando na surface
Game.Instance.Renderer.SetRenderTarget(surface);
Draw.FilledCircle(4, 32, new Vector2(32), Color.Black, Color.White);
Game.instance.Renderer.SetRenderTarget(null);
```

## Fontes
Quando criadas manualmente, fontes são baseadas em sprites.

```csharp
// Using
using Claw;
using Claw.Graphics;

// Definindo campos
private SpriteFont mono, custom;

// Criando fonte - MonoSpace
Vector2 spacing = new Vector2(0, 2); // Espaçamento (caractere, linha)
Vector2 charSize = new Vector2(16); // Tamanho dos caracteres
mono = new SpriteFont(TextureAtlas.Sprites["Atlas/Fonte"], spacing, charSize, 'A', 'B', 'C', 'D' /* Demais caracteres */);
//mono = new SpriteFont(TextureAtlas.Sprites["Atlas/Fonte"], spacing, charSize, "ABCD");

// Criando fonte - Tamanho customizado
Dictionary<char, SpriteFont.Glyph> glyphs = new Dictionary<char, SpriteFont.Glyph>();
glyphs.Add('A', new SpriteFont.Glyph(new Rectangle(0, 0, 12, 16)));
custom = new SpriteFont(TextureAtlas.Sprites["Atlas/Fonte"], Vector2.Zero, glyphs);
```

## Áudios
```csharp
// Using
using System;
using Claw;
using Claw.Audio;

// Criando áudio
float[] samples = new float[360];

/*
    Preencha o array aqui (valores entre -1 a 1)
    Áudios Stereo são organizados em:
    sample[0] = Esquerda
    sample[1] = Direita
    ...
    --------------------------------------------
    Já áudios Mono:
    sample[0] = Sample
    sample[1] = Sample
    ...
    No play, o sample será divido em dois
*/

SoundEffect effect = new SoundEffect(Channels.Mono, samples);
```