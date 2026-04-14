**Fecha:** 2026-04-14  
**Asignatura:** Estructuras de Datos / Algoritmos
**Estudiante:** Daniel Esteban Romero Dueñes 
**Codigo:** 2250948  
**Tema:** Árboles de Huffman y Compresión de Datos

## 1. Introducción

Los árboles de Huffman son una estructura de datos utilizada en informática para la compresión de información sin pérdida. Este método fue desarrollado por David A. Huffman en 1952 y es ampliamente utilizado en diferentes formatos de compresión de archivos.

## 2. ¿Qué son los Árboles de Huffman?

Un árbol de Huffman es un árbol binario que se construye a partir de la frecuencia de aparición de los símbolos en un conjunto de datos. Su objetivo es asignar códigos binarios más cortos a los símbolos más frecuentes y códigos más largos a los menos frecuentes, reduciendo así el tamaño total de los datos.

## 3. ¿Cómo funciona?

El algoritmo de Huffman sigue los siguientes pasos:

1. **Frecuencia:** Se calcula la frecuencia de cada símbolo.
2. **Nodos:** Se crean nodos para cada símbolo con su frecuencia.
3. **Cola de prioridad:** Se seleccionan los dos nodos con menor frecuencia.
4. **Combinar nodos:** Se combinan en un nuevo nodo cuya frecuencia es la suma de ambos.
5. **Repetir:** Se repite el proceso hasta formar un único árbol.

## 4. Codificación

Una vez construido el árbol:

- Se asigna **0** a cada rama izquierda.
- Se asigna **1** a cada rama derecha.

Cada símbolo obtiene un código binario único, sin ambigüedades.

### Ejemplo:

| Símbolo | Código |
|--------|--------|
| A      | 0      |
| B      | 10     |
| C      | 110    |
| D      | 111    |
## 5. Ejemplo práctico

Texto de ejemplo:AAAAABBBC
Frecuencias:

- A: 5
- B: 3
- C: 1

Codificación posible:

- A → 0
- B → 10
- C → 11

Resultado comprimido: 000001010101011

## 6. Aplicaciones

Los árboles de Huffman se utilizan en:

- Compresión de archivos (ZIP)
- Formato de imágenes (JPEG)
- Codificación de datos
- Transmisión eficiente de información

## 7. Ventajas

- Reduce el tamaño de los datos
- No pierde información (compresión sin pérdida)
- Es eficiente y óptimo

## 8. Conclusión

Los árboles de Huffman son una herramienta fundamental en la compresión de datos. Gracias a su eficiencia, permiten optimizar el almacenamiento y la transmisión de información, siendo una técnica clave en la informática moderna.