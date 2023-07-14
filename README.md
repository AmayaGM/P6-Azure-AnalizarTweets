# Practica 6 con "Azure Logic"

*Analizar tweets con Azure Logic*

**Paso 1 _Functions_**
- Poner en la barra de busqueda "logic" y elegir la opcion de "logic apps"
![Paso 1](/imagenes/img1.png)

**Paso 2 _Crear App logic_**
- Primero debemos elegir el boton "Crear" 
![Paso 2](/imagenes/img2.png)

- Ir a datos basicos
  ![Paso 2.1](/imagenes/img2_1.png)

  - Debemos elegir en detalles del proyecto:
      - La suscripcion
      - El grupo de recursos previamente creado
      ![Paso 2.2](/imagenes/img2_2.png)

  - Debemos elegir en detalles de instancia:
      - Nombre con el que queremos llamar la aplicacion
      - La region donde deseamos crearla
      - Elegir si habilitar Log Analytics
      ![Paso 2.3](/imagenes/img2_3.png)

  - Debemos elegir el tipo de plan
      ![Paso 2.4](/imagenes/img2_4.png)
  - Debemos elegir en Redundancia de zona
        ![Paso 2.5](/imagenes/img2_5.png)

- Dar en revisar y crear
  ![Paso 2.6](/imagenes/img2_6.png)

- Dar en crear e ir al recurso
  ![Paso 2.7](/imagenes/img2_7.png)

- Crear una aplicacion logica en blanco
    ![Paso 2.8](/imagenes/img2_8.png)

- Buscar y elegir Twitter. Posteriormente presionar en cuando se publica un nuevo tweet
    ![Paso 2.9.1](imagenes/img2_9.png)

- Iniciar sesión en twitter
    ![Paso 2.10](imagenes/img2_10.png)

- LLenar el formulario con los datos correspondientes 
  - Texto de busqueda (poner el # que queremos analizar)
  - Especificar el intervalo de tiempo con el que queremos que analice (en este caso cada 5 seg)
![Paso 2.11](/imagenes/img2_11.png)
  - Al finalizar dar en nuevo paso

- Ingresamos en el buscador la palabra "text" y elegimos Azure cognitive
![Paso 2.12](/imagenes/img2_12.png)

- Despues elegimos sentimientos
![Paso 2.13](/imagenes/img2_13.png)

>Nota: Ir al paso 3 cognitive services

- Pegamos la clave y la url del paso 3 en nuestro formulario, por ultimo damos en crear
![Paso 2.14](/imagenes/img2_14.png)

- A continuacion deberemos poner un id al documento que corresponde al tweet y despues decir lo que se analizara que en este caso sera el texto para despues dar en agregar una accion
![Paso 2.15](/imagenes/img2_15.png)

- Buscamos la hoja de calculo de google y elegimos insertar fila
![Paso 2.16](/imagenes/img2_16.png)
![Paso 2.16.1](/imagenes/img2_16_1.png)

- Iniciamos sesión en google
![Paso 2.17](/imagenes/img2_17.png)

- Elegimos una hoja de calculo creada previamente en google drive, a continucacion ligamos cada fila con su contenido y agregamos un paso
![Paso Hc](/imagenes/img_hc_.png)
![Paso 2.18](/imagenes/img2_18.png)

- Escogemos la opcion "publicar mensaje en un chat o  canal" e iniciamos sesión en nuestro teams
![Paso 2.19](/imagenes/img2_19.png)

- LLenamos las casillas correspondientes y guardamos lo que hemos realizado
![Paso 2.20](/imagenes/img2_20.png)

>Nota: Ir al paso 4

      
**Paso 3 Cognitive services**
- Poner en la barra de busqueda "cognitive services" y elegir la opcion 
![Paso 3](imagenes/img3.png)

- Crear un servicio de lenguaje
  ![Paso 3.1](/imagenes/img3_1.png)

  - Debemos elegir en detalles del proyecto:
      - La suscripcion
      - El grupo de recursos previamente creado
      ![Paso 3.2](/imagenes/img2_2.png)
  - Debemos elegir en detalles de instancia:
      - Nombre 
      - La region donde deseamos crearla
      - Plan de tarifa
      ![Paso 3.3](/imagenes/img3_2.png)
    
- Dar en revisar y crear, finalmente creamos 
  ![Paso 3.4 y 3.5](/imagenes/img3_3.png)

- Vamos a claves y puntos de conexion
  ![Paso 3.6](/imagenes/img3_4.png)

- Copiamos la primera clave y la url, despues regresamos al paso 2
  ![Paso 3.7](/imagenes/img3_5.png)

**Paso 4 Parte final**
- Una vez guardado la ultima parte del paso 2 dar en ejecutar encadenador
![Paso 4](imagenes/img4.png)

- Al checar excel podemos observar el resultado de nuestro analisis
![Paso 4.1](imagenes/img4_1.png)

- Al checar Teams tambien podemos observar el resultado de nuestro analisis
![Paso 4.2](imagenes/img4_2.png)
