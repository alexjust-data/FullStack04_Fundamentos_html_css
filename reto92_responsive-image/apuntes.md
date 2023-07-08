
**Responsive images**

Las "Responsive images" o "imágenes responsivas" son imágenes que se adaptan al tamaño y orientación de la pantalla del dispositivo que está visualizando la página web. Esto se hace para optimizar la experiencia del usuario, ya que las imágenes de tamaño adecuado se ven mejor y cargan más rápido que las imágenes que son demasiado grandes o pequeñas para la pantalla.

Las imágenes responsivas son una parte esencial del diseño web responsivo, una filosofía de diseño y desarrollo que se esfuerza por garantizar que las páginas web se vean y funcionen bien en una variedad de dispositivos y tamaños de pantalla.

Existen varias técnicas para crear imágenes responsivas: 

* se puede utilizar el atributo `srcset` en HTML5, que permite especificar varios archivos de imagen y las condiciones (como la resolución de la pantalla) en las que se debería usar cada uno.

* Otra opción es usar CSS para cambiar el tamaño de las imágenes según las características de la pantalla del dispositivo. Con el uso de las consultas de medios (`Media Queries`), puedes definir estilos diferentes para diferentes condiciones, como anchos de pantalla específicos.

Es importante destacar que el uso de imágenes responsivas no solo mejora la experiencia del usuario, sino que también puede tener un impacto en el SEO, ya que los motores de búsqueda pueden penalizar los sitios web que no están optimizados para dispositivos móviles.

---

Ambos <picture> y <srcset> son elementos HTML que se utilizan para adaptar las imágenes en diseño web responsive, pero se utilizan de maneras ligeramente diferentes y tienen diferentes niveles de soporte en los navegadores.

El elemento <picture> se utiliza con múltiples elementos <source> cada uno con un atributo media que define la consulta de media (media query) bajo la cual esa imagen específica se debe mostrar. El navegador seleccionará la primera <source> que coincida con la consulta de medios actual. Si ninguna coincide, o si el navegador no soporta <picture>, utilizará el elemento <img> como fallback. Esto te da mucho control sobre qué imagen mostrar en función de las características del dispositivo.

Por otro lado, el atributo srcset en el elemento <img> le permite al navegador seleccionar la imagen más apropiada basada en la densidad de píxeles del dispositivo y el tamaño de la ventana del navegador. Puedes proporcionar varias imágenes y decir al navegador la resolución de cada una de ellas (utilizando w para ancho en píxeles o x para densidad de píxeles), y el navegador elegirá la más adecuada. No tienes que proporcionar consultas de medios explícitas como en <picture>.

Por tanto, la principal diferencia es que <picture> te da un control más explícito sobre qué imagen se debe mostrar en función de las características del dispositivo, mientras que srcset permite al navegador tomar la decisión en función de la resolución de las imágenes y las condiciones actuales de visualización.

Por último, un detalle a tener en cuenta es que a pesar de que <picture> y srcset son compatibles con la mayoría de los navegadores modernos, puede haber algunas excepciones, especialmente con navegadores más antiguos. Es siempre una buena práctica verificar la compatibilidad del navegador y proporcionar alternativas cuando sea necesario.


**Recursos**:
* https://www.responsivebreakpoints.com/ 
* https://caniuse.com/
