# Texture
```csharp
public class Texture
```
Representa uma textura no jogo.<br />
## Texture
```csharp
public Texture(int width, int height) { }
```
## Texture
```csharp
public Texture(int width, int height, uint[] pixels) { }
```
## Width
```csharp
public readonly int Width;
```
## Height
```csharp
public readonly int Height;
```
## Pixel
```csharp
public static Texture Pixel { get; internal set; } 
```
## Size
```csharp
public Claw.Vector2 Size { get; } 
```
## BlendMode
```csharp
public Claw.Graphics.BlendMode BlendMode { get; set; } 
```
## SetData
```csharp
public virtual void SetData(uint[] pixels) { }
```
Altera os pixels desta textura.<br />
