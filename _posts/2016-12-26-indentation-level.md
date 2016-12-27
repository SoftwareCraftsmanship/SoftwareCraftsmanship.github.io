# Nivel de indentación

Mantén el número de niveles de indentación de tus funciones *muy* bajo. El [estilo de programación del Kernel de Linux](https://www.kernel.org/doc/html/latest/process/coding-style.html#indentation) recomienda mantener tu nivel de indentación por debajo de 3:

> ... The answer to that is that if you need more than 3 levels of indentation, you're screwed anyway, and should fix your program.

Por favor, evita

```
public void MiFunction()
{
    for (int i = 0; i < 100; i++)
    {
        if (something)
        {
            if (something)
            {
                if (something)
                {
                    if (something)
                    {
                        if (something)
                        {
                            //...
                        }
                    }
                }
            }
        }
    }
}
```

