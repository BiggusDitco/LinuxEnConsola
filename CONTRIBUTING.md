# Guía de Contribución a LinuxEnConsola

¡Gracias por tu interés en colaborar con **LinuxEnConsola**! 🎉 
 
Este proyecto busca crear una lista en español de programas útiles para la consola de Linux.  

La idea es que sea claro, colaborativo y fácil de usar.  

---

## 🛠️ Cómo contribuir

Podés colaborar de dos formas:

1. **Agregando un programa nuevo**
   - Editá el archivo de la categoría correspondiente (`sistema.md`, `red.md`, `utilidades.md`, etc.).
   - Usá el siguiente formato:

     ```markdown
     ### `nombre_del_programa`
     Breve descripción en una o dos líneas.  
     ```bash
     comando_de_ejemplo
     ```

   - Ejemplo:

     ```markdown
     ### `curl`
     Herramienta para transferir datos desde o hacia un servidor.  
     ```bash
     curl https://ejemplo.com
     ```

2. **Sugiriendo mejoras**
   - Podés abrir un **Issue** si querés proponer un programa, reportar un error o mejorar la organización.

---

## 🚀 Flujo de trabajo con GitHub

1. Hacé un **fork** de este repositorio.  
2. Creá una rama para tu aporte:  
   ```bash
   git checkout -b agregar-nuevo-programa
    ```
3. Realizá los cambios en el archivo correspondiente.
4. Guardá y confirmá los cambios:
   ```bash
   git add .
   git commit -m "Agrego programa: nombre_del_programa"
   ```
5. Subí tu rama:
   ```bash
   git push origin agregar-nuevo-programa
   ```
6. Abrí un Pull Request desde tu fork hacia este repositorio. 🎉

## ✅ Reglas básicas

* Escribir en español neutro.
* Una sola herramienta por Pull Request (para mantenerlo simple de revisar).
* Descripción breve y clara (sin copiar/pegar páginas enteras del manual).
* Siempre que sea posible, incluir un ejemplo mínimo de uso.

## 💡 Consejo

Si nunca hiciste un Pull Request en GitHub, no te preocupes: este proyecto también es un lugar para aprender.
Podés practicar, equivocarte y volver a intentarlo sin problema.

Gracias por sumar tu conocimiento a LinuxEnConsola 🙌
