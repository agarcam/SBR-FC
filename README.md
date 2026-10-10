# Sistema de Inferencia Basado en Reglas y Factores de Certeza

## Descripción

Este proyecto desarrolla un sistema de inferencia basado en reglas que permite obtener conclusiones a partir de una base de conocimientos y un conjunto de hechos iniciales. Para gestionar la incertidumbre, utiliza factores de certeza comprendidos entre -1 y 1, que representan el grado de confianza asociado a cada hecho y regla.

El sistema implementa un mecanismo de **encadenamiento hacia atrás (*backward chaining*)**, que parte de una meta y analiza las reglas necesarias para determinar su grado de certeza.

## Funcionalidades

- **Motor de inferencia:** resolución de metas mediante encadenamiento hacia atrás.
- **Gestión de incertidumbre:** cálculo y propagación de factores de certeza.
- **Base de conocimientos:** definición de reglas y sus correspondientes factores de certeza.
- **Base de hechos:** almacenamiento de hechos iniciales y sus niveles de confianza.
- **Procesamiento de reglas:** análisis de expresiones mediante la biblioteca `regex` de C++.
- **Casos de prueba:** distintos escenarios para comprobar el funcionamiento del sistema y los resultados de la inferencia.

## Tecnologías utilizadas

- C++
- Biblioteca estándar de C++ (`regex`)
- Sistema de reglas de producción
- Factores de certeza para el razonamiento bajo incertidumbre

## Organización del proyecto

```text
.
├── Pruebas/
│   ├── prueba1/
│   ├── prueba2/
│   ├── prueba3/
│   └── pruebaA/
└── Software/
    ├── SBR-FC.cpp
    ├── ejecutable.exe
    └── ManualDeUso.pdf
```

- `Pruebas/`: contiene los escenarios de evaluación, los ficheros de entrada y la documentación asociada.
- `Software/`: incluye el código fuente, el ejecutable y el manual de uso.

## Ejecución

El programa recibe dos ficheros como argumentos:

```bash
./programa BC.txt BH.txt
```

- `BC.txt`: contiene las reglas de inferencia y sus factores de certeza.
- `BH.txt`: contiene los hechos iniciales y sus respectivos factores de certeza.

Los nombres de los ficheros y del ejecutable deben adaptarse a los disponibles en cada caso de prueba.

## Objetivo

El objetivo es aplicar técnicas de inteligencia artificial simbólica para construir un sistema capaz de razonar con información incierta, evaluar distintas reglas y calcular el grado de confianza de las conclusiones obtenidas.

