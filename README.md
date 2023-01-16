# CS_DepuracionInteractivaDeApp.NET-E2

Ejercicio: Registro y seguimiento

****Registro y seguimiento****

En la parte superior del archivo `Program.cs`
, agregaremos una nueva instrucción `using`
 para incorporar `System.Diagnostics`
 de forma que podamos usar los métodos `Debug`
.

```csharp
using System.Diagnostics;
```

Agregue una instrucción `WriteLine`
 al principio del método `Fibonacci`
 para una mayor claridad al depurar el código.

```csharp
Debug.WriteLine($"Entering {nameof(Fibonacci)} method");
Debug.WriteLine($"We are looking for the {n}th number");
```

Al final de nuestro bucle `for`
, podríamos imprimir cada valor. O bien, podríamos usar una instrucción de impresión condicional con `WriteIf`
 o `WriteLineIf`
. Agregue una línea de impresión solo cuando `sum`
 sea 1 al final del bucle "for".

```csharp
for (int i = 2; i <= n; i++)
{                  
    sum = n1 + n2;
    n1 = n2;
    n2 = sum;
    Debug.WriteLineIf(sum == 1, $"sum is 1, n1 is {n1}, n2 is {n2}");    
}
```

Ejecute la aplicación y verá la siguiente salida:

Resultado

```
Entering Fibonacci method
We are looking for the 5th number
sum is 1, n1 is 1, n2 is 1
```

