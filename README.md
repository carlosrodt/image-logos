Este repositorio ha sido creado para facilitar el acceso a imágenes de calidad para desarrolladores que trabajan con Docker. 
Las imágenes están organizadas en diferentes categorías para que puedas encontrar fácilmente lo que necesitas.

## Imágenes disponibles

Las imágenes se encuentran en las siguientes categorías:

*  Contiene Logos de marcas conocidas y genéricos.
*  Objetos  Imágenes de objetos cotidianos y abstractos.
*  Iconos de Apps  Iconos y capturas de pantalla de aplicaciones.
*  Ilustraciones, Dibujos y gráficos para decorar tus proyectos.
*  Fondos: Imágenes de fondo para presentaciones y aplicaciones.

Puedes explorar las imágenes en las diferentes carpetas del repositorio. Cada imagen tiene un nombre descriptivo para que puedas identificarla fácilmente.

## Uso con Docker

Puedes utilizar estas imágenes en tus proyectos Docker de varias formas:

-- Despliega el contenedor y utilizar las rutas de las imagenes en los proyectos y apps propias.

-- Copiar las imagenes requeridas en los proyecos.

-- Creando una imagen base:** Puedes crear una imagen personalizada a partir de este proyecto y luego utilizar esta imagen como base para tus otros proyectos.

##  Ejemplo de docker yaml
version: "3.9"  

services:
  image-logos-srv:  # Nombre del servicio (puedes cambiarlo)
    build: .  # Construye la imagen desde el Dockerfile en el directorio actual
    ports:
      - "30045:30045"  # Mapea el puerto 30045 del host al puerto 30045 del contenedor
     volumes:  
       - ./datos:/app/datos
       - ./config:/app/config
    
