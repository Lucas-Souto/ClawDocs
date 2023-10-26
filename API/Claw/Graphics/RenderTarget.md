# RenderTarget
```csharp
public sealed class RenderTarget : Texture
```
Representa um alvo de renderização para o [Renderer](/API/Claw/Graphics/Renderer.md#Renderer) .<br />
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
Recomendado: Use o método [Renderer](/API/Claw/Graphics/Renderer.md#Renderer) no lugar disso.<br />
<br />
