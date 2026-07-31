# Entregables adicionales

## Generador de datos de prueba

El proyecto utiliza un generador de datos para crear información de prueba con las siguientes cantidades:

- 1000 usuarios
- 10000 productos
- 100000 interacciones

Estos datos permiten evaluar el funcionamiento del sistema y realizar pruebas de rendimiento.

---

## Resultados de las recomendaciones

El sistema genera una lista ordenada de recomendaciones para cada usuario considerando:

- Categorías preferidas.
- Categorías bloqueadas.
- Historial de compras.
- Productos consultados.
- Calificación del producto.
- Disponibilidad en inventario.
- Etiquetas relacionadas.

Cada recomendación incluye la puntuación obtenida y las razones por las cuales fue seleccionada.

---

## Reporte generado

El sistema genera un reporte con información como:

- Total de productos analizados.
- Total de recomendaciones.
- Puntuación promedio.
- Recomendaciones por categoría.
- Productos rechazados.
- Causas de rechazo.
- Productos más populares.

El reporte puede exportarse en formato JSON, CSV o TXT.

---

## Comparación de rendimiento: List vs Sequence

Se realizó una comparación utilizando conjuntos de datos grandes.

### List
- Procesa todos los elementos de manera inmediata.
- Mayor consumo de memoria.
- Adecuado para colecciones pequeñas.

### Sequence
- Procesamiento perezoso (lazy).
- Menor consumo de memoria.
- Mejor rendimiento para grandes volúmenes de datos.

Para este proyecto, `Sequence` resultó la alternativa más eficiente al trabajar con miles de productos e interacciones.
