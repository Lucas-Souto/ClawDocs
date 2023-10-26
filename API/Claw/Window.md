# Window
```csharp
public sealed class Window
```
Representa a janela do jogo.<br />
## ClientResized
```csharp
public System.EventHandler ClientResized;
```
É executado sempre que o tamanho da janela é alterado, independentemente de quem causou essa mudança.<br />
## MouseVisible
```csharp
public bool MouseVisible { get; set; } 
```
## Borderless
```csharp
public bool Borderless { get; set; } 
```
## FullScreen
```csharp
public bool FullScreen { get; set; } 
```
## CanUserResize
```csharp
public bool CanUserResize { get; set; } 
```
## IsActive
```csharp
public bool IsActive { get; } 
```
Diz se a janela está em foco (selecionada).<br />
## IsMouseFocused
```csharp
public bool IsMouseFocused { get; } 
```
Diz se o mouse está dentro da janela.<br />
## IsFocused
```csharp
public bool IsFocused { get; } 
```
Diz se o mouse está dentro da janela e ela está em foco (selecionada).<br />
## Title
```csharp
public string Title { get; set; } 
```
## Location
```csharp
public Claw.Vector2 Location { get; set; } 
```
## Size
```csharp
public Claw.Vector2 Size { get; set; } 
```
## Finalize
```csharp
protected virtual void Finalize() { }
```
## Dispose
```csharp
public virtual void Dispose() { }
```
## Centralize
```csharp
public void Centralize() { }
```
Centraliza a janela.<br />
## SetMousePosition
```csharp
public void SetMousePosition(Claw.Vector2 position) { }
```
Altera a posição do mouse, relativo a janela.<br />
