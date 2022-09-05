# RealidadVirtual2022-VR-CardboardOfficialExample

Ejemplo base oficial de Google Cardboard

Para compilar, hay configuración adicional que deben realizar antes de probar el ejemplo oficial en sus dispositivos, en este repositorio YA ESTÁ TODO CONFIGURADO Y LISTO, sin embargo les dejo los pasos a seguir si lo quieren hacer desde cero. 

Empezando por los Publish Settings ya que es necesario crear un custom template para Gradle, indicamos la siguiente configuración: 

![Publish settings](https://github.com/DiegoTovar/RealidadVirtual2022-VR-CardboardOfficialExample/blob/main/Captura2.PNG)

Les aparecerá una carpeta Plugins dentro de Assets, hay que modificar 2 archivos de la siguiente manera:

- gradleTemplate.properties

link de este archivo en el repo: https://github.com/DiegoTovar/RealidadVirtual2022-VR-CardboardOfficialExample/blob/main/Cardboard/Assets/Plugins/Android/gradleTemplate.properties

- mainTemplate.gradle

link de este archivo en el repo: https://github.com/DiegoTovar/RealidadVirtual2022-VR-CardboardOfficialExample/blob/main/Cardboard/Assets/Plugins/Android/mainTemplate.gradle

----------

El Plugin de cardboard ya no es compatible con Mono, por lo que deben configurar el uso de IL2CPP con ARM64 en Other Settings:

![Other settings](https://github.com/DiegoTovar/RealidadVirtual2022-VR-CardboardOfficialExample/blob/main/Captura.PNG)

----------

Por último deben actualizar el target API level a 31 o mayor, aquí dejo 2 formas de hacerlo

- Método 1: descargando directamente el SDK

tutorial: https://www.youtube.com/watch?v=oro-e252Ezs

link de descarga de los sdk: https://androidsdkmanager.azurewebsites.net/SDKPlatform

- Método 2: mediante Android Studio

tutorial: https://www.youtube.com/watch?v=O3AHZVEDAQY

link de descarga de Android Studio: https://developer.android.com/studio?hl=es-419&gclid=Cj0KCQjwmdGYBhDRARIsABmSEeNMzUw4A1-XxQ8l92Uoljfcrw9tFPLXNVCXQ0k__NgoooBlmquhe7IaAg-IEALw_wcB&gclsrc=aw.ds


Una vez actualizado el SDK configuramos el target API Level en Unity dentro de la sección Other Settings:

![API Level](https://github.com/DiegoTovar/RealidadVirtual2022-VR-CardboardOfficialExample/blob/main/Captura4.PNG)



Cuando intenten compilar, si Unity lo solicita, hagan click en actualizar el SDK:

![Update](https://github.com/DiegoTovar/RealidadVirtual2022-VR-CardboardOfficialExample/blob/main/Captura3.PNG)

Si siguieron los pasos anteriores podrán generar su propio apk (también incluido en este repo si lo quieren instalar directamente), para mayor información acerca de los pasos anteriores les dejo la documentación oficial:

link de la guía de inicio rápido: https://developers.google.com/cardboard/develop/unity/quickstart

----------

BONUS:

![BONUS](https://github.com/DiegoTovar/RealidadVirtual2022-VR-CardboardOfficialExample/blob/main/BONUS.png)
