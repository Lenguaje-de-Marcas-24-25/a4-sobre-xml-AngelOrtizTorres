# UD1 A5 Sobre XML

**1. Indica las características propias del lenguaje XML.**
   
XML (eXtensible Markup Language) es un metalenguaje que permite definir etiquetas personalizadas y es utilizado para la representación de datos de forma estructurada. Sus características principales incluyen:

   - Extensibilidad: Permite definir etiquetas y estructuras según las necesidades.

   - Legibilidad humana y máquina: Los documentos XML son fáciles de leer para las personas y máquinas.

   - Independencia de plataforma: XML es independiente de plataformas y lenguajes de programación.

   - Formato auto-descriptivo: Los datos y la estructura se describen en el propio documento​.

**2. Identifica la estructura de un documento XML y sus reglas sintácticas.**

Un documento XML tiene una estructura jerárquica. Las reglas básicas de un documento XML incluyen:

- Debe comenzar con una declaración XML (opcional) como <?xml version="1.0" encoding="UTF-8"?>.

- Debe tener un único elemento raíz que contenga todos los demás elementos.

- Las etiquetas deben estar bien anidadas.

- Los atributos deben estar siempre entre comillas.

- Los nombres de etiquetas y atributos son sensibles a mayúsculas

**3. En XML qué es un nodo raíz**

El nodo raíz es el elemento principal que contiene todos los elementos de un documento XML. Es el contenedor superior que agrupa todo el contenido y cada documento XML debe tener solamente un nodo raíz.

**4. Indica qué es un elemento vacío. Ejemplos**

Un elemento vacío en XML es aquel que no tiene contenido ni elementos internos. Se puede representar de dos maneras:

- Forma larga: ``<elemento></elemento>``
- Forma corta o auto-cerrada: ``<elemento />``

Un ejemplo podría ser: 
`<imagen />`
// Este ejemplo está en forma corta.


**5. Qué sentido tiene crear documentos XML bien formado.**

Crear documentos bien formados es esencial para garantizar que:

- Los datos puedan ser intercambiados de manera segura y precisa.
- Cualquier aplicación que interprete XML pueda procesarlo correctamente.
- Los datos sean legibles tanto por humanos como por máquinas​

**6. Qué es un espacio de nombres. Ventajas de uso.**

Un espacio de nombres (namespace) en XML es una forma de evitar conflictos de nombres cuando se combinan diferentes vocabularios XML. Se definen utilizando un prefijo asociado a una URI única.

Ventajas de su uso:

- Evita conflictos entre elementos o atributos que tienen el mismo nombre.
- Permite combinar diferentes documentos XML sin ambigüedades.

**7. Entidades en XML. Crea un XML con las entidades vistas en clase.**

Las entidades en XML son una forma de representar caracteres especiales o secuencias de texto reutilizables.

```XML
<!DOCTYPE ejemplo [
  <!ENTITY lt "<">
  <!ENTITY gt ">">
]>
<documento>
    Comparar con: &lt; imagen /&gt;.
</documento>

```

**8. Comentarios en XML. Muestra uno de los ejercicios anteriores con el enunciado dentro de un comentario. Dentro del comentario deben aparecer dos guiones.**

Los comentarios en XML se utilizan para añadir información o notas sin afectar el contenido del documento. Se escriben dentro de ``<!-- -->``.
```XML
<!--7. Entidades en XML. Crea un XML con las entidades vistas en clase.-->

<contenido>Las entidades en XML son una forma de representar caracteres especiales o secuencias de texto reutilizables.</contenido>
```

