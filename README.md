MODELO C4

El modelo C4 es un enfoque visual para documentar y comunicar la arquitectura de software de forma clara y estructurada. 
Un buen diagrama de arquitectura de software facilita la comunicación a los equipos de desarrollo y producto, la idea principal es que los diagramas puedan ser entendidos e interpretados por equipos técnicos y no técnicos.

Cuenta con cuatro niveles de abstracción, de ahí su nombre:
	Nivel 1: Diagrama de Contexto. 
	Nivel 2: Diagrama de Contenedores
	Nivel 3: Diagrama de Componentes
	Nivel 4: Diagrama de Código (opcional)
Estos permiten mejorar la documentación de proyectos completos a fin de que la audiencia pueda comprender en que consiste, como esta conformado y como se interrelaciona con otros sistemas o servicios.

 
Ejercicio Práctico.

Realizaremos un Análisis y Diagramas de un Sistema de Banca Electrónica Web de un banco X, considerando los siguientes aspectos:
1.	Solo puede ser accedido por clientes del banco
2.	Cuenta con un esquema de autenticación y autorización (Azure Entra ID)
3.	Cuenta con un modelo de factor de autenticación mediante OTP (Contraseña de un Solo Uso) que se enviará al teléfono celular del usuario como SMS o Push Notification, o email
4.	La OTP tiene un tiempo de vigencia de 3 minutos, caso contrario caduca y deniega el acceso
5.	Valida que el usuario se encuentre activo en el banco
6.	El sistema permite consultar Posición Consolidada y Estados de Cuenta
7.	Permite consultar y actualizar cupos para transacciones y pagos de las cuentas de clientes
8.	Permite realizar transferencias bancarias e interbancarias
9.	Permite realizar pagos de servicios con debido a cuenta
10.	Envía un mensaje al usuario (cliente) como SMS o Push Notification, o email, cuando se ha realizado una transacción bancaria
11.	Permite guardar los logs de sistema y transaccionales en un repositorio como Elasticsearch.
