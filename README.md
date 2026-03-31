# Proyecto-Comportamiento-de-sus-clientes-Sprint-2
Este proyecto representa la culminación de la fase de análisis descriptivo para Store 1. Tras asegurar la calidad de la información en el primer sprint, este segundo módulo se enfoca en transformar los datos crudos en insights accionables sobre el comportamiento, preferencias y niveles de lealtad de los usuarios.
📝 Descripción del Proyecto
1. El Dataset: Dimensiones del Cliente
Trabajamos con una estructura de datos anidada que incluye:

Identidad: IDs únicos y nombres (previamente normalizados).

Demografía: Edad del usuario (convertida a tipo entero para análisis estadístico).

Intereses: Categorías de productos preferidas (Electrónica, Deportes, Libros, etc.).

Finanzas: Desglose de gastos por categoría, permitiendo calcular el Lifetime Value (LTV) inicial del cliente.

2. Metodología y Pipeline de Datos
El análisis se ejecutó a través de un flujo de trabajo optimizado en Python:

Estandarización Profunda: Aplicación de lógica de limpieza a gran escala, eliminando caracteres especiales (guiones bajos) y espacios en blanco en los nombres de todos los registros.

Procesamiento de Listas Anidadas: Uso de bucles e iteraciones para navegar por las sublistas de gastos y categorías, transformando datos complejos en métricas simples.

Lógica de Segmentación: Implementación de condicionales para identificar a los "High Spenders" (clientes con gasto total > $1000) y usuarios con intereses específicos.

Automatización de Reportes: Generación de cadenas de texto dinámicas (f-strings) que resumen el perfil de cada cliente de forma legible para el equipo directivo.

🚀 Hallazgos Clave (Insights)
De la muestra analizada de 6 clientes estratégicos, se determinó lo siguiente:

Segmento Premium: El 50% de la muestra (Mike Reed, Samantha Smith y Emily Brown) califican como clientes de alto valor al superar los $1000 de gasto total.

Perfil del Top Spender: El usuario 32415 (Mike Reed) lidera el gasto con un total de $1280, concentrado principalmente en Electrónica y Deportes.

Diversidad de Intereses: A pesar de la variedad, la categoría HOME aparece frecuentemente en usuarios con gastos moderados, sugiriendo una oportunidad de "cross-selling".
