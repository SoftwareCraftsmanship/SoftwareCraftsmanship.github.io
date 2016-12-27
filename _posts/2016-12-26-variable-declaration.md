# Declaración de variables

Una variable dentro de una función debe ser declarada antes de su primer uso, por favor evita tener una función extensa o super extensa con todas las declaraciones y las inicializaciones en las primeras líneas de la función. Esto provocará desplazamientos entre el uso de la variable y su declaración o inicialización.

Por favor, evita:

```
public void DoSomething()
{
    int a, b, c;
    double d, e, f;

    // blah, blah, blah
    // 100 lines of code later

    if (a > 1)
        DoSomething();

    // 100 lines of code more

    if (b != 0.0)   
        DoSomethingElse();
}
```

Es mejor:

```
public void DoSomething()
{
    int a = 0;
    // Some action to update a
    if (a > 1)
        DoSomething();
}
```
