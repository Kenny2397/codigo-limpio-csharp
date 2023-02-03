# codigo-limpio-csharp
Buenas prácticas y código limpio en C#

## Buenas Prácticas

Estándares comprobados y verificados
Resuelven desafíos de escenarios comunes
Brindan guías fáciles de aprender y comprender
Permiten tener una estructura similar para múltiples proyectos
## Código Limpio

Un código que sigue las buenas prácticas
Código fácil de entender y analizar
Código fácil de mantener
Código fácil de actualizar
Código fácil de escalar
Cómo lo logramos

## Mantener bajo acoplamiento
Utilizar sintaxis simple y moderna
Evitar incorporar muchas librerías de terceros
Distribución de responsabilidades
Creación de componentes pequeños
## Deuda técnica - Technical debt

Se refiere a los problemas técnicos que puede tener un software que son adquiridos durante la fase de desarrollo y que deben ser solucionados en el futuro.
Puede estar presente en cualquier aspecto de una aplicación como: Seguridad, rendimiento, escalabilidad, etc.
A veces puede resultar más costosa que el mismo desarrollo.
## Refactoring

Proceso de cambios sobre un código para el mejoramiento en cualquier aspecto (rendimiento, seguridad, legibilidad, etc.)
Lo más importante es hacer cambios manteniendo la lógica de negocio sin afectaciones.
Debe ser recurrente.
Disminuye la deuda técnica a futuro.

# .NET Vs .NET CORE VS .NET FRAMEWORK
> .Net Framwork (2001)
Solo Compatible con Windows
Plataforma de ejección intermedia
C#, VBNET, F#, Visual C++
Aplicaciones corporativas con arquitectura tradicional
Visual Studio
> .Net Core (2016)

Multiplataforma
C#, F# y VB
Orientado a la nube, alto rendimiento y aplicaciones en capas
Sin dependencia de IDE
> .NET Core = .NET

# Ventajas de .NET
Aplicaciones web
y web APIs
usando ASP.NET.
Aplicaciones Web
usando Web
assembly con
Blazor.
Multiplataforma.
● Compatible con múltiples lenguajes de
programación.
● Muchas herramientas y librerías gratuitas. 
● Evolución y mejoras.
● Apoyo de la comunidad y documentación.
● Soporte continuo.
● Integración con servicios Microsoft.
● Retrocompatibilidad.

# Common language runtime CLR

Transforma de Common Intermediate
Language (CIL) o MSIL a Código nativo.

Compilador en tiempo de ejecución.

Agiliza la ejecución del código compilado.

# ¿Qué es Roslyn?
.NET Compiler Platform.
C# y Visual Basic.
Rápido y Ágil.
Analiza estilo y calidad del codigo.
Open Source
Integrado por defecto en Visual Studio y al dotnet CLI.

# Common Language Specification:

Es un conjunto de reglas y métricas básicas que necesitan seguir y cumplir los lenguajes compatibles con .NET para luego ser compilados(Roslyn) a otro lenguaje neutral intermedio llamado CIL (Common Intermediate Language) donde finalmente será traducido al CLR (Common Language Runtime) que dará como resultado un lenguaje Assembly, lenguaje máquina.

El CLS asegura la completa interoperabilidad entre las aplicaciones, independientemente del lenguaje utilizado para crear la aplicación.

# Common Type System
Common Type System

Define los tipos generales que se usan dentro del lenguaje compatible con .NET.
Provee la librería base para los tipos primitivos (byte, char, int).
Provee un modelo de tipos orientado a objetos.

# Instalando el SDK
sdk .net LTS
WSL puede usar este tutorial
( https://www.dotnetthailand.com/programming-cookbook/wsl-powershell-useful-scripts/install-dotnet )

# dotnet CLI
dotnet run 
dotnet build
dotnet restore
dotnet watch run 

# 📁⚙ Archivos de compilación
ㅤ

Dentro del proceso de compilación tenemos dos carpetas relacionadas
ㅤ
📁 bin : Contiene el archivo compilado del proyecto .dll y más

📁 obj : Tiene los archivos que se generan en la compilación de manera temporal, par despues ser entregado al archivo bin.
ㅤ
| 💡 Para limpiar la compilación hecha, podemos usar el comando dotnet clean
ㅤ

Existen dos modos de compilación en .NET
ㅤ
modo debug
Prepara la aplicación para el uso en un ámbito de pruebas, suele ser un poco más pesado que el modo de compilado release. Se recomienda no usar este compilado en modo producción, ya que se puede exponer información que solo nos interesa que se muestre cuando estamos probando y no así cuando nuestros clientes lo ejecuten.
ㅤ
modo release

Prepara la aplicación para que esté lista en producción, tenga un mejor performance y rendimiento, además de que sea mucho más liviano. Elimina todos los archivos que no se necesitan en producción.

# el comando que nos permite compilar a producción es
dotnet build --configuration release
Ideas/conceptos claves
ㅤ

.dll: es un archivo que viene una compilación de un lenguaje de alto nivel (ej. C#)
ㅤ
.exe: es un archivo ejecutable que únicamente se utiliza en Windows, resumiendo su funcionamiento toma el archivo .dll y lo ejecuta en nuestro ordenador.

# Archivo globaljson
dotnet new globaljson


