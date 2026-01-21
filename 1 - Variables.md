### Declaración
Para declarar una variable en C# es necesario indicar primero que nada el tipo de dato, seguido el nombre de la variable. 

En este ejemplo declaramos una variable de tipo `int` de nombre `x`:
```cs
namespace CSharpCourse
{
    internal class Program
    {
        static void Main(string[] args)
        {
            int x; // Declaración
        }
    }
}
```

### Inicialización
Para asignar un valor se llama a la variable y mediante el signo de igualación se indica el valor que contendrá la variable:
```cs
namespace CSharpCourse
{
    internal class Program
    {
        static void Main(string[] args)
        {
            int y = 999; // Declaración e inicialización
        }
    }
}
```

### Declaración e inicialización
También es posible declarar y asignar un valor al mismo tiempo:
```cs
namespace CSharpCourse
{
    internal class Program
    {
        static void Main(string[] args)
        {
            int y = 999; // Declaración e inicialización
        }
    }
}
```

### Imprimir valores en consola
Para imprimir el valor en la consola se utiliza el método `Console.WriteLine()`, en IDEs como Visual Studio se puede utilizar el shortcut `cw` + `Enter` para autocompletar el método sin tener que escribirlo completo.
```cs
namespace CSharpCourse
{
    internal class Program
    {
        static void Main(string[] args)
        {
            int y = 999;
			
            Console.WriteLine(y); // 999
        }
    }
}
```

### Declaración e inicialización de variables a partir de otras variables
Podremos declarar variables que puedan contener un valor derivado como una suma (en el caso del tipo de dato `int`).
```cs
namespace CSharpCourse
{
    internal class Program
    {
        static void Main(string[] args)
        {
	        int x = 888;
            int y = 999;
            int z = x + y;
			
            Console.WriteLine(z); // 1887
        }
    }
}
```

### Nombres de variables descriptivos
Recuerda que en programación los nombre de las variables deben ser descriptivos, especialmente es útil en el paradigma de Programación Orientada a Objetos. Cómo ejemplo vamos a declarar una variable que contenga una edad:
```cs
namespace CSharpCourse
{
    internal class Program
    {
        static void Main(string[] args)
        {
	        int edad = 23;
			
            Console.WriteLine(edad); // 23
        }
    }
}
```

### Concatenación
A veces será necesario imprimir en consola texto que contenga en si el valor de alguna variable, la técnica básica para esto se le conoce como **concatenación de variables**. Consiste en escribir el texto que deseamos ver en la terminal y además con un signo de suma "concatenar" la variable que deseamos leer:
```cs
namespace CSharpCourse
{
    internal class Program
    {
        static void Main(string[] args)
        {
	        int edad = 23;
			
            Console.WriteLine("Mi edad es: " + edad); // Mi edad es: 23 
        }
    }
}
```

### Tipos de datos
Además del tipo de dato `int` es posible declarar variables de distintos tipos, entre ellos tenemos `float` que es el más utilizado a la hora de requerir números decimales. Como ejemplo vamos a declarar una variable que contenga una altura:
```cs
namespace CSharpCourse
{
    internal class Program
    {
        static void Main(string[] args)
        {
	        double altura = 1.70;
	        Console.WriteLine("Mi altura es: " + altura); // Mi altura es 1.7 
        }
    }
}
```

Otro tipo de dato es `bool` que se utiliza para asignar valores como `true` o `false`. En este caso vamos a declarar una variable que contenga un `bool` que diga si estamos graduados o no:
```cs
namespace CSharpCourse
{
    internal class Program
    {
        static void Main(string[] args)
        {
            bool estaGraduado = false;
            Console.WriteLine(estaGraduado); // False
        }
    }
}
```


El siguiente tipo de dato es `char` se utiliza para almacenar un único caracter y específicamente debe ser escrito con comillas simples, de lo contrario C# arrojará una excepción.
```cs
namespace CSharpCourse
{
    internal class Program
    {
        static void Main(string[] args)
        {
            char signoDolar = '$';
            Console.WriteLine(signoDolar); // $
        }
    }
}
```

Para declarar textos completos se utiliza `string`, al contrario de `char` aquí es obligatorio utilizar comillas dobles:
```cs
namespace CSharpCourse
{
    internal class Program
    {
        static void Main(string[] args)
        {
            string holaMundo = "¡Hola Mundo!";
            Console.WriteLine(holaMundo); // ¡Hola Mundo!
        }
    }
}
```