# GameObject
```csharp
public class GameObject
```
A classe base dos objetos.<br />
## GameObject
```csharp
public GameObject() { }
```
## DontDestroy
```csharp
public bool DontDestroy;
```
## Name
```csharp
public string Name;
```
## Colliders
```csharp
public System.Collections.Generic.List<Claw.Polygon> Colliders;
```
## Opacity
```csharp
public float Opacity;
```
## Color
```csharp
public Claw.Color Color;
```
## Flip
```csharp
public Claw.Graphics.Flip Flip;
```
## InstantlyAdd
```csharp
public static bool InstantlyAdd;
```
Com essa opção desativada, será necessário adicionar o objeto aos componentes do jogo manualmente.<br />
## UpdateOrder
```csharp
public virtual int UpdateOrder { get; set; } 
```
## DrawOrder
```csharp
public virtual int DrawOrder { get; set; } 
```
## Enabled
```csharp
public virtual bool Enabled { get; set; } 
```
## Visible
```csharp
public virtual bool Visible { get; set; } 
```
## Game
```csharp
public Claw.Game Game { get; } 
```
## Exists
```csharp
public bool Exists { get; } 
```
## Parent
```csharp
public GameObject Parent { get; set; } 
```
## Tags
```csharp
public string[] Tags { get; } 
```
## Children
```csharp
public GameObject[] Children { get; } 
```
## Rotation
```csharp
public float Rotation { get; set; } 
```
## Position
```csharp
public Claw.Vector2 Position { get; set; } 
```
## Scale
```csharp
public Claw.Vector2 Scale { get; set; } 
```
## RotationInParent
```csharp
public float RotationInParent { get; set; } 
```
## PositionInParent
```csharp
public Claw.Vector2 PositionInParent { get; set; } 
```
## ScaleInParent
```csharp
public Claw.Vector2 ScaleInParent { get; set; } 
```
## Facing
```csharp
public Claw.Vector2 Facing { get; } 
```
## Origin
```csharp
public virtual Claw.Vector2 Origin { get; set; } 
```
## Sprite
```csharp
public virtual Claw.Graphics.Sprite Sprite { get; set; } 
```
## SpriteArea
```csharp
public virtual Claw.Rectangle? SpriteArea { get; set; } 
```
## Animator
```csharp
public Claw.Animator Animator { get; set; } 
```
## EnabledChanged
```csharp
public event System.EventHandler<System.EventArgs> EnabledChanged;
```
## UpdateOrderChanged
```csharp
public event System.EventHandler<System.EventArgs> UpdateOrderChanged;
```
## DrawOrderChanged
```csharp
public event System.EventHandler<System.EventArgs> DrawOrderChanged;
```
## VisibleChanged
```csharp
public event System.EventHandler<System.EventArgs> VisibleChanged;
```
## Finalize
```csharp
protected virtual void Finalize() { }
```
## Initialize
```csharp
public virtual void Initialize() { }
```
É executado quando o componente é adicionado ao jogo.<br />
## Dispose
```csharp
protected virtual void Dispose(bool disposing) { }
```
## Dispose
```csharp
public virtual void Dispose() { }
```
## AddTag
```csharp
public void AddTag(string tag) { }
```
Adiciona uma tag no objeto.<br />
**tag**: Case insensitive.<br />
## RemoveTag
```csharp
public void RemoveTag(string tag) { }
```
Remove uma tag do objeto.<br />
**tag**: Case insensitive.<br />
## HasTag
```csharp
public bool HasTag(string tag) { }
```
Diz se este [GameObject](/API/Claw/GameObject#GameObject) possui uma tag específica.<br />
## Step
```csharp
public virtual void Step() { }
```
## Render
```csharp
public virtual void Render() { }
```
## Destroy
```csharp
protected void Destroy(GameObject gameObject, bool runDestroy) { }
```
Destrói um objeto.<br />
## SelfDestroy
```csharp
public void SelfDestroy(bool runDestroy) { }
```
Destrói o objeto.<br />
## OnDestroy
```csharp
protected virtual void OnDestroy() { }
```
Chamado quando o objeto é destruído.<br />
## OnEnabledChanged
```csharp
protected virtual void OnEnabledChanged(object sender, System.EventArgs args) { }
```
Chamado quando o [GameObject.Enabled](/API/Claw/GameObject#Enabled) muda. Usado pelo evento [GameObject.EnabledChanged](/API/Claw/GameObject#EnabledChanged) .<br />
**sender**: Este componente.<br />
**args**: Argumentos para o evento.<br />
## OnUpdateOrderChanged
```csharp
protected virtual void OnUpdateOrderChanged(object sender, System.EventArgs args) { }
```
Chamado quando o [GameObject.UpdateOrder](/API/Claw/GameObject#UpdateOrder) muda. Usado pelo evento [GameObject.UpdateOrderChanged](/API/Claw/GameObject#UpdateOrderChanged) .<br />
**sender**: Este componente.<br />
**args**: Argumentos para o evento.<br />
## OnVisibleChanged
```csharp
protected virtual void OnVisibleChanged(object sender, System.EventArgs args) { }
```
Chamado quando o [GameObject.Visible](/API/Claw/GameObject#Visible) muda.<br />
**sender**: Este componente.<br />
**args**: Argumentos para o evento.<br />
## OnDrawOrderChanged
```csharp
protected virtual void OnDrawOrderChanged(object sender, System.EventArgs args) { }
```
Chamado quando o [GameObject.DrawOrder](/API/Claw/GameObject#DrawOrder) muda.<br />
**sender**: Este componente.<br />
**args**: Argumentos para o evento.<br />
