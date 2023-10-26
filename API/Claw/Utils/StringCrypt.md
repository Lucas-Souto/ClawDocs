# StringCrypt
```csharp
public static class StringCrypt
```
## Crypt
```csharp
public static string Crypt(string text, bool encrypt, int amount) { }
```
Criptografa/Descriptografa um texto.<br />
**encrypt**: True para criptografia e false para descriptografia.<br />
**amount**: Senha para a criptografia/descriptografia.<br />
## Crypt
```csharp
public static string Crypt(string text, bool encrypt, int[] amount) { }
```
Criptografa/Descriptografa um texto.<br />
**encrypt**: True para criptografia e false para descriptografia.<br />
**amount**: Sequência para a criptografia/descriptografia.<br />
## Crypt
```csharp
public static string Crypt(string text, bool encrypt, string password) { }
```
Criptografa/Descriptografa um texto.<br />
**encrypt**: True para criptografia e false para descriptografia.<br />
**password**: Senha da criptografia.<br />
## StringToBinary
```csharp
public static string StringToBinary(string text) { }
```
Converte texto para binário.<br />
## BinaryToString
```csharp
public static string BinaryToString(string bynary) { }
```
Converte binário para texto.<br />
## StringToHex
```csharp
public static string StringToHex(string text) { }
```
Converte um texto para hex.<br />
## HexToString
```csharp
public static string HexToString(string hex) { }
```
Converte hex para texto.<br />
## AllCrypt
```csharp
public static string AllCrypt(string text, bool encrypt, int amount) { }
```
Usa os métodos Crypt, StringToBinary/BinaryToString e StringToHex/HexToString para criptografar/descriptografar um texto.<br />
**encrypt**: True para criptografia e false para descriptografia.<br />
**amount**: Senha para a criptografia/descriptografia.<br />
## AllCrypt
```csharp
public static string AllCrypt(string text, bool encrypt, int[] amount) { }
```
Usa os métodos Crypt, StringToBinary/BinaryToString e StringToHex/HexToString para criptografar/descriptografar um texto.<br />
**encrypt**: True para criptografia e false para descriptografia.<br />
**amount**: Sequência para a criptografia/descriptografia.<br />
## AllCrypt
```csharp
public static string AllCrypt(string text, bool encrypt, string password) { }
```
Usa os métodos Crypt, StringToBinary/BinaryToString e StringToHex/HexToString para criptografar/descriptografar um texto.<br />
**encrypt**: True para criptografia e false para descriptografia.<br />
**password**: Senha da criptografia.<br />
