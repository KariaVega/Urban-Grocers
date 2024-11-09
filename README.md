# Proyecto: Urban-Grocers
![image](https://github.com/user-attachments/assets/43ce7d9a-083e-470a-ae8d-869b46fbe672)

### :page_facing_up: *Documentación utilizada:* 
- Requisitos para el back-end de Urban Grocers: [Link de Requisitos](https://practicum-content.s3.us-west-1.amazonaws.com/new-markets/qa-sprint-3/QA_3.1.1_Requisitos_para_el_back-end_de_Urban.grocers.pdf)
- Dirección del servidor: [Link de aplicacion](https://3cd0a718-aa1b-46c4-86bd-318797f0fda9.containerhub.tripleten-services.com)
- Apidocs, documentación de la API:  [Link de Apidocs](https://cnt-345fbc31-54d8-4931-9fe1-6c8fd4c12c2d.containerhub.tripleten-services.com/docs/)


### 🛠️ *Lenguajes y herramientas utilizadas:*
<div id="header" align="left">
    
- Jira: Registro y seguimiento de errores.
- Apidocs: Revisión de documentación de API's
- Postman: Pruebas manuales.
- HTTP: protocolo.
- REST: estructura.
- JSON: Formato para solicitudes REST.
- Diseño de pruebas para la API.
- MS Office: Documentación de las pruebas.
  
</a>
<img decoding="async" src="https://img.shields.io/badge/Jira-0052CC?style=for-the-badge&logo=Jira&logoColor=white" alt="Jira"/>
<img decoding="async" src="https://img.shields.io/badge/Apidocs-darkblue?style=for-the-badge&logo=Apidocs&logoColor=white" alt="Apidocs"/>
<img decoding="async" src="https://img.shields.io/badge/Postman-D83B01?style=for-the-badge&logo=Postman&logoColor=white" alt="Postman"/>
<img decoding="async" src="https://img.shields.io/badge/HTTP-D80B01?style=for-the-badge&logo=HTTP&logoColor=white" alt="HTTP"/>
<img decoding="async" src="https://img.shields.io/badge/REST-black?style=for-the-badge&logo=REST&logoColor=white" alt="REST"/>
<img decoding="async" src="https://img.shields.io/badge/JSON-purple?style=for-the-badge&logo=JSON&logoColor=white" alt="JSON"/>
<img decoding="async" src="https://img.shields.io/badge/Microsoft_Office-D86B01?style=for-the-badge&logo=microsoft-office&logoColor=white" alt="microsoft-office"/>
</a>

### :fireworks: *Descripción del Backend (API) Urban Grocers*
- El área de desarrollo ha agregado una nueva función en la API de Urban.Grocers, así que pasaron una nueva versión de la API para que la pruebes. La aplicación permite realizar pedidos y entrega de productos por catalogo.
Para la revisión del Banckend, se realizó una lista de comprobación de los elementos con un total de 134 items. Se ejecutaron las pruebas manuales del aplicativo, utilizando solicitudes HTTP y en formato JSON para gestionar pedidos y entregas, comprobando la funcionalidad. A continuación, se enlistan las pruebas con sus especificaciones de cada una de ellas.

### :paw_prints: *Pasos a seguir para la ejecución de las pruebas:* 

- Conexión al servidor medienta la URL.
- Analisis de requisitos.
- Elaboración de lista de comprobación.
- Protocolo HTTP
- Solicitudes en formato JSON.
- Estructura REST
- Ejecución de las pruebas.

### :page_facing_up: *Lista de Comprobación de Pruebas:*  
- Endpoints probados

  - [POST] /api/v1/kits (Crear kit vacio) Campo **Name**
  - [POST] /api/v1/kits (Crear kit vacio) Campo **cardId**
  - [POST] /api/v1/kits/{id}/products (Agregar comestibles al carrito ) Campo **URL {id}**
  - [POST] /api/v1/kits/{id}/products (Agregar comestibles al carrito ) Cuerpo de la solicitud "productsList" Campo **{id}**
  - [POST] /api/v1/kits/{id}/products (Agregar comestibles al carrito ) Cuerpo de la solicitud "productsList" Campo **{quantity}** 
  - [PUT]  /api/v1/orders/:id (La capacidad de agregar comestibles al carrito) Campo **URL {id}**
  - [PUT]  /api/v1/orders/:id (La capacidad de agregar comestibles al carrito) Cuerpo de la solicitud "productsList" Campo **{id}**
  - [PUT]  /api/v1/orders/:id (La capacidad de agregar comestibles al carrito) Cuerpo de la solicitud "productsList" Campo **{quantity}** 
  - [GET]  /api/v1/orders/:id (obtener una lista de productos que se han agregado al carrito ) Campo **URL {id}**
  - [DELETE]   /api/v1/orders/:id (La capacidad de eliminar el carrito) Campo **URL {id}**
  - [POST]  /order-and-go/v1/delivery (la capacidad de comprobar si el servicio de entrega Order and Go está disponible y cuánto cuesta) Comprobando rango de peso en relación al costo de **"order and go disponibilidad y costo"** 


### 🧪 *Resultados de las pruebas:* 
 La documentación de las pruebas se desarrollo en los siguientes archivos disponibles.
 
#### :file_folder: Documentación para el Backend (*API*):
  - Proyecto de automatización: -  [Link de automatización de las pruebas](https://github.com/KariaVega/qa-project-Urban-Grocers-app-es) 
  - Listas de comprobación: - [Link de Lista de comprobación](https://docs.google.com/spreadsheets/d/1Fq5p6_TYopFFrb-cHdXnNJeiVfkebj5y/edit?usp=sharing&ouid=117701476691019254617&rtpof=true&sd=true)
  - Reporte y seguimiento de errores: - [Link de Reporte de Errores](https://arqkarvga.atlassian.net/issues/?jql=project+%3D+%22KV1G4SIDE%22+ORDER+BY+created+DESC&atlOrigin=eyJpIjoiNDQwNzRlNmRlODk3NDkyYmFlNTA1ZDFkNzEwMzFkZjMiLCJwIjoiaiJ9)

### :page_facing_up: *Resumen del informe:* 
 - Informe del producto:

Se realizaron las pruebas del producto Urban Grocers, algunas de las fallas se encuentran en la creación de kit, los datos de entrada no cumplen con los requisitos y sus parámetros. Otras funciones importantes que fallan son las de eliminación de carritos, una de las funciones principales que afectan de manera directa el funcionamiento de la app. Finalmente los cálculos de los costos del servicio de entrega, no corresponden a los establecidos en los requisitos, algunos de los parámetros y sus restricciones, no concuerdan con los costos y el horario disponible en relación al número de productos y su peso. Por lo que se notifica un estado no aprobado y de corrección. 
   
<div id="header" align="center"> 
  
![image](https://github.com/user-attachments/assets/53cbe0da-08d5-4a40-af07-c484873119d1)
 
 

