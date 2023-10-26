# Vector3
```csharp
public struct Vector3
```
Descreve um vetor 3D.<br />
## Vector3
```csharp
public Vector3(float x, float y, float z) { }
```
## Vector3
```csharp
public Vector3(float value) { }
```
## Vector3
```csharp
public Vector3(Claw.Vector2 vector2, float z) { }
```
## X
```csharp
public float X;
```
## Y
```csharp
public float Y;
```
## Z
```csharp
public float Z;
```
## Zero
```csharp
public static Vector3 Zero { get; } 
```
X: 0; Y: 0; Z: 0.<br />
## One
```csharp
public static Vector3 One { get; } 
```
X: 1; Y: 1; Z: 1.<br />
## Normalize
```csharp
public void Normalize() { }
```
Transforma este [Vector3](/API/Claw/Vector3#Vector3) em um vetor de unidade com a mesma direção.<br />
## Clamp
```csharp
public static Vector3 Clamp(Vector3 value, Vector3 min, Vector3 max) { }
```
Retorna um vetor que respeite os limites mínimo e máximo.<br />
## Distance
```csharp
public static float Distance(Vector3 a, Vector3 b) { }
```
Retorna a distância entre dois vetores.<br />
## Normalize
```csharp
public static Claw.Vector2 Normalize(Claw.Vector2 value) { }
```
Transforma um [Vector3](/API/Claw/Vector3#Vector3) em um vetor de unidade com a mesma direção.<br />
## Lerp
```csharp
public static Vector3 Lerp(Vector3 a, Vector3 b, float amount) { }
```
Realiza a interpolação linear entre dois vetores.<br />
**a**: Valor atual.<br />
**b**: Valor alvo.<br />
**amount**: Valor de ponderação (entre 0 e 1).<br />
## DeltaLerp
```csharp
public static Vector3 DeltaLerp(Vector3 a, Vector3 b, float amount, bool scaled) { }
```
Realiza a interpolação linear entre dois vetores, usando delta time.<br />
**a**: Valor atual.<br />
**b**: Valor alvo.<br />
**amount**: Valor de ponderação.<br />
**scaled**: Se o delta time será [Time.DeltaTime](/API/Claw/Time#DeltaTime) (true) ou [Time.UnscaledDeltaTime](/API/Claw/Time#UnscaledDeltaTime) (false).<br />
## Approach
```csharp
public static Vector3 Approach(Vector3 value, Vector3 target, float shift) { }
```
Incrementa um valor por um determinado deslocamento, mas nunca além do valor final.<br />
## Approach
```csharp
public static Vector3 Approach(Vector3 value, Vector3 target, Vector3 shift) { }
```
Incrementa um valor por um determinado deslocamento, mas nunca além do valor final.<br />
## ToString
```csharp
public virtual string ToString() { }
```
Retorna uma string representando este vetor 3D no formato:
            {X:[ [Vector3.X](/API/Claw/Vector3#X) ] Y:[ [Vector3.Y](/API/Claw/Vector3#Y) ] Z:[ [Vector3.Z](/API/Claw/Vector3#Z) ]}<br />
## operator +
```csharp
public static Vector3 operator +(Vector3 a, Vector3 b) { }
```
## operator -
```csharp
public static Vector3 operator -(Vector3 a, Vector3 b) { }
```
## operator -
```csharp
public static Vector3 operator -(Vector3 value) { }
```
## operator *
```csharp
public static Vector3 operator *(Vector3 a, Vector3 b) { }
```
## operator *
```csharp
public static Vector3 operator *(Vector3 a, float b) { }
```
## operator *
```csharp
public static Vector3 operator *(float a, Vector3 b) { }
```
## operator /
```csharp
public static Vector3 operator /(Vector3 a, Vector3 b) { }
```
## operator /
```csharp
public static Vector3 operator /(Vector3 a, float b) { }
```
## operator /
```csharp
public static Vector3 operator /(float a, Vector3 b) { }
```
## operator ==
```csharp
public static bool operator ==(Vector3 a, Vector3 b) { }
```
## operator !=
```csharp
public static bool operator !=(Vector3 a, Vector3 b) { }
```
