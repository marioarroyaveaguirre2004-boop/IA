# 1. Nombre del Space

**Nombre:** Image Studio

**Enlace:** [https://huggingface.co/spaces/nsfwalex/ImageStudio](https://huggingface.co/spaces/nsfwalex/ImageStudio)

---

## 2. ¿Qué hace el agente?

El agente, a partir de un prompt, genera una imagen con un formato ya sea realista o en formato anime.

---

## 3. Análisis PEAS

- **P (Performance):** La imagen generada es fiel con el prompt, además debe ser bastante agradable a la vista o seguir los lineamientos opcionales de configuración.
- **E (Environment):** La interfaz, el chat de prompts, las configuraciones avanzadas, el botón de opción de formatos.
- **A (Actuators):** El botón para empezar a generar y el motor de generación.
- **S (Sensors):** El sensor de formatos y el chat de prompts.

---

## 4. Clasificación del entorno

- **Observable:** Parcial — el agente solo genera a partir de un prompt; es una caja negra para los usuarios, ya que no se ve el proceso ni tiene acceso total a todo nuestro pensamiento, por eso en modelos como estos hay que ser súper específico.
- **Determinista:** No — como opera por semillas, el mismo prompt puede generar muchas imágenes distintas.
- **Episódico:** Sí — es una ejecución independiente cada vez.
- **Estático:** Sí — el agente no cambia de criterio en medio de la ejecución, solo sigue un prompt.
- **Discreto:** No — hay aspectos del proceso que son continuos, como píxeles y valores de color.
- **Conocido:** Sí — las reglas de funcionamiento del modelo son conocidas por el usuario, aunque el resultado exacto no sea predecible.

---

## 5. ¿Qué tipo de programa de agente creen que es?

Es de **reflejo simple**, porque toma el prompt actual y directamente genera la imagen, sin usar historial ni estado interno, ya que el entorno es episódico. No construye nada más allá de lo que se le pide; simplemente aplica una función fija entrada → salida.

