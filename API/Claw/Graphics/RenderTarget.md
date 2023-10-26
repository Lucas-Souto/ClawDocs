# RenderTarget
```csharp
public sealed class RenderTarget : Claw.Graphics.Texture
```
Representa um alvo de renderização para o [Renderer](/API/Claw/Graphics/Renderer#Renderer) .<br />
## RenderTarget
```csharp
public RenderTarget(int width, int height) { }
```
## SetData
```csharp
public virtual void SetData(uint[] pixels) { }
```
Altera os pixels desta textura.<br />
Aviso: Uso não recomendado (cada pixel será atualizado manualmente, num laço de repetição).<br />
Recomendado: Use o método [Renderer](/API/Claw/Graphics/Renderer#Renderer) no lugar disso.<br />
<br />