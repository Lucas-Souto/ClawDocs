# TextureAtlas
```csharp
public static class TextureAtlas
```
Representa um texture atlas.<br />
## Sprites
```csharp
public static System.Collections.ObjectModel.ReadOnlyDictionary<string,Claw.Graphics.Sprite> Sprites;
```
## CurrentPage
```csharp
public static Claw.Graphics.Texture CurrentPage { get; internal set; } 
```
Qual a última [Sprite.Texture](/API/Claw/Graphics/Sprite#Texture) usada pelo [Draw](/API/Claw/Graphics/Draw#Draw) .<br />
## AddSprite
```csharp
public static void AddSprite(Claw.Graphics.Sprite sprite) { }
```
Adiciona uma sprite ao [TextureAtlas.Sprites](/API/Claw/Graphics/TextureAtlas#Sprites) .<br />
Aviso: O primeiro pixel da sua textura deve ser um pixel branco.<br />
<br />
## AddSprites
```csharp
public static void AddSprites(Claw.Graphics.Sprite[] sprites) { }
```
Adiciona sprites ao [TextureAtlas.Sprites](/API/Claw/Graphics/TextureAtlas#Sprites) .<br />
Aviso: O primeiro pixel da sua textura deve ser um pixel branco.<br />
<br />
