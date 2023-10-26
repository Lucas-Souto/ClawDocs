# Renderer
```csharp
public sealed class Renderer
```
Representa o renderizador da [Window](/API/Claw/Window#Window) .<br />
## ClearColor
```csharp
public Claw.Color ClearColor { get; set; } 
```
## Finalize
```csharp
protected virtual void Finalize() { }
```
## Dispose
```csharp
public virtual void Dispose() { }
```
## GetRenderTarget
```csharp
public Claw.Graphics.RenderTarget GetRenderTarget() { }
```
Retorna o alvo da renderização atual.<br />
## SetRenderTarget
```csharp
public void SetRenderTarget(Claw.Graphics.RenderTarget renderTarget) { }
```
Altera o alvo da renderização.<br />
**renderTarget**: Nulo para desenhar na [Window](/API/Claw/Window#Window) .<br />
## DrawTexture
```csharp
public void DrawTexture(Claw.Graphics.Texture texture, Claw.Rectangle source, Claw.Rectangle destination, Claw.Color color, Claw.Vector2 origin, float angle, Claw.Graphics.Flip flip) { }
```
Desenha uma imagem.<br />
**angle**: Graus.<br />
## Clear
```csharp
public void Clear() { }
```
Limpa a tela com o [Renderer.ClearColor](/API/Claw/Graphics/Renderer#ClearColor) .<br />
