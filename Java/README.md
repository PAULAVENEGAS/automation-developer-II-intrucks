# Prueba Técnica – Java (InTrucks)

Bienvenido/a. Esta prueba evalúa conocimientos de Java orientados a lógica, APIs, manejo de JSON, colecciones, manejo de archivos, y conceptos básicos de programación orientada a objetos.

Por favor crea tu solución en este mismo repositorio siguiendo la estructura propuesta, o puedes reorganizarla si tienes una estructura propia siempre que sea clara.

---

## 📌 Ejercicio 1 – Manejo de colecciones y lógica

**Objetivo:** Evaluar lógica básica, colecciones, y estructuras de datos.

### Instrucción
Escribe un programa en Java que:

1. Reciba esta lista de números enteros:  
   `10, 20, 20, 10, 30, 40, 10, 30`
2. Imprima:  
   - La cantidad de veces que cada número aparece.  
   - El número que más se repite.  
   - El número que menos se repite.

### Ejemplo de salida
```
10 → 3 veces
20 → 2 veces
30 → 2 veces
40 → 1 vez

Número que más se repite: 10
Número que menos se repite: 40
```

---

## 📌 Ejercicio 2 – Consumo de API + JSON + Exportar CSV

**Objetivo:** Evaluar uso de librerías, consumo de APIs, JSON, manejo de errores e I/O.

### Instrucción

Consumir la API pública:

🔗 https://dummyjson.com/products

Tu programa debe:

1. Hacer solicitud GET a `/products`.
2. Validar el código HTTP (manejar errores).
3. Convertir la respuesta JSON a objetos Java (Gson o Jackson).
4. Filtrar productos por categoría (ejemplo: `"smartphones"`).
5. Exportar los productos filtrados a un archivo CSV:  
   `output/resultados.csv`

### Estructura sugerida
- `Ejercicio2.java` → lógica principal  
- `Producto.java` → clase POJO  
- `CsvExporter.java` → exportación CSV  

---

## 📌 Ejercicio 3 – CRUD básico (sin frameworks)

**Objetivo:** Evaluar OOP, clases, estructuras y lógica CRUD.

### Instrucción

Crear un CRUD simple para la clase:

```java
class Usuario {
    int id;
    String nombre;
    String email;
}
```

Debes implementar métodos para:

- Crear usuar
