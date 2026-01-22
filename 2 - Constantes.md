Las constantes son un tipo de dato que no se puede modificar. Usualmente las utilizamos en datos que nunca cambian. Por ejemplo, vamos a suponer que necesitamos el valor de la gravedad, si nosotros no definimos la variable como una constante, alguien más puede modificar su valor, generando así problemas de seguridad y errores en nuestros resultados.
```cs
namespace CSharpCourse
{
    internal class Program
    {
        static void Main(string[] args)
        {
            double gravedad = 9.8;
            gravedad = 100;
        }
    }
}
```

Para solucionar esto utilizaremos la palabra reservada `const` antes del tipo de dato de la variable para convertirla en una constante.
```cs
namespace CSharpCourse
{
    internal class Program
    {
        static void Main(string[] args)
        {
            const double gravedad = 9.8; // Convirtiendo a constante
            gravedad = 100; // Error
            Console.WriteLine(gravedad);
        }
    }
}
```

De esta forma si alguien intenta cambiar el valor de una constante obtendrá el siguiente error: `La parte izquierda de una asignación debe ser una variable, una propiedad o un indizador`.

Las constantes siempre deben ser inicializadas con un valor al momento de su declaración, de lo contrario obtendremos el error: `El campo const requiere que se proporcione un valor`.
```cs
namespace CSharpCourse
{
    internal class Program
    {
        static void Main(string[] args)
        {
            const double gravedad; // Error
            Console.WriteLine(gravedad);
        }
    }
}
```