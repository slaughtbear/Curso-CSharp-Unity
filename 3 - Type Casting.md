El concepto de `type casting` trata sobre la conversión de un tipo de dato a otro. Esto es útil para diferentes tipos de casos.

Por ejemplo, supongamos que tenemos una variable de tipo `double` que almacena como valor `9.8` que representa a la gravedad. ¿Es posible convertir este dato a un entero? la respuesta es sí, esto se logra mediante el método `Convert.ToInt32()`.
```cs
namespace CSharpCourse
{
    internal class Program
    {
        static void Main(string[] args)
        {
            double gravedad = 9.8;
            int entero = Convert.ToInt32(gravedad);
            Console.WriteLine(entero); // 10
        }
    }
}
```

> [!NOTE]
>  Al realizar una conversión de tipo con este método se redondea al número más cercano, es decir, en este caso el valor inicial era `9.8` y al aplicar la conversión el nuevo valor entero es `10`. Lo mismo sucedería para `9.2` en donde si se aplica la conversión el resultado sería `9`.

En C# para saber de qué tipo de dato es una variable se utiliza el método `GetType()`:
```cs
namespace CSharpCourse
{
    internal class Program
    {
        static void Main(string[] args)
        {
            double gravedad = 9.8;
            int entero = Convert.ToInt32(gravedad);
            Console.WriteLine(entero.GetType()); // System.Int32
        }
    }
}
```

# Métodos de conversión
Estos son sólo algunos de los métodos de conversión, existen aún más en C#:
1. `ToString()`: Convierte un tipo de dato a string.
2. `ToBoolean()`: Convierte un tipo de dato a bool.
3. `ToChar()`: Convierte un tipo de dato a char.