-- ¿Qué es el DNS y para qué sirve?
DNS son las iniciales de Domain Name System (sistema de nombres de dominio) y es una tecnología basada en una base de datos que sirve para resolver nombres en las redes, es decir, para conocer la dirección IP de la máquina donde está alojado el dominio al que queremos acceder.

-- ¿Que es la resolucion de dominio y para que virve?
Es el proceso de mapear dominios legibles para seres humanos
La resolución de nombres de dominio permite navegar por Internet utilizando nombres de dominio en lugar de direcciones numéricas.

El Servicio de Informática y Comunicaciones presta un doble servicio:

Al usuario final: ofrecer los servidores para que puedan navegar por Internet.
A los administradores de servidores: publicar en Internet los nombres de sus máquinas para que sean accesibles.

-- ¿Que son los dominios y subdominios?
Un subdominio es una forma de tener un sitio (web) relacionado, como anexo, a una web principal.
Los subdominios son del tipo: http://subdominio.dominio.com, éstos apuntan realmente a una carpeta del propio alojamiento que has contratado, pero mostrando su contenido desde el subdominio.

-- ¿Que son las busqueda de dominio DNS?
Las zonas de búsqueda DNS son divisiones organizativas del espacio de nombres DNS que contienen información específica sobre dominios 2. Cada zona representa un nivel en la jerarquía de nombres DNS y contiene registros relacionados con los dominios bajo ese nivel.

Las zonas de búsqueda DNS sirven para organizar y gestionar eficientemente el sistema de nombres de dominio, permitiendo que los dispositivos puedan comunicarse usando nombres legibles por humanos en lugar de direcciones IP numéricas. Estas zonas dividen el espacio de nombres DNS en segmentos manejables, contienen información específica sobre dominios, dan autoridad a los administradores y facilitan la resolución de nombres. Además, permiten la propagación de cambios y mejoran el rendimiento de la resolución de nombres al facilitar consultas directas entre servidores autoritativos dentro del mismo espacio de nombres. 


-- Tipos de servidores DNS y sus funciones principales:

Servidor DNS recursivo: Primera parada para consultas recursivas, puede responder con información de caché o reenviar consultas.
Servidor DNS autoritativo: Contiene información definitiva sobre dominios específicos, proporciona respuestas directamente.
Servidor DNS de raíz: Contiene información sobre dominios de nivel superior más altos, reenvía consultas al servidor autoritativo correspondiente.
Resolutor de código auxiliar: Se encuentra en dispositivos finales y realiza consultas DNS para aplicaciones.
Estos servidores trabajan juntos en una cadena de consultas para traducir nombres de dominio en direcciones IP, permitiendo que los usuarios accedan fácilmente a sitios web usando nombres legibles en lugar de direcciones numéricas.


-- ¿Que son los registros DNS?
Los registros DNS son archivos de mapeo que indican a los servidores DNS a qué dirección IP corresponde un dominio particular. Sus principales funciones son:

Traducir nombres de dominio en direcciones IP, permitiendo acceder a sitios web usando nombres legibles.
Definir servidores de correo electrónico (MX).
Indicar servidores autorizados para un dominio (NS).
Crear aliases para dominios existentes (CNAME).
Mapear direcciones IP a nombres de dominio (PTR).
Definir información de contacto y administrativa para un dominio (SOA).
Estos registros permiten configurar cómo se alojan sitios web, qué servidores de correo se utilizan y cómo se manejan otras funcionalidades de dominios en Internet.


-- Funcionamiento de consulta recursiva

Una consulta recursiva DNS es un proceso en el cual un servidor DNS recursivo busca información sobre un dominio específico siguiendo una serie de pasos. Su principal función es permitir que los usuarios accedan a sitios web utilizando nombres legibles en lugar de direcciones IP numéricas.

-- Funciones principales de una consulta recursiva DNS:

Busca información sobre dominios específicos.
Verifica primero la caché local del servidor recursivo.
Consulta a servidores de raíz si no hay información en caché.
Reenvía la consulta al servidor autoritativo apropiado para el dominio.
Recibe y devuelve la respuesta final al dispositivo original.
Esta consulta recursiva es fundamental para que los usuarios puedan acceder fácilmente a sitios web usando nombres legibles en lugar de direcciones numéricas. Es un proceso infinito que continúa hasta obtener una respuesta definitiva, característica propia de consultas recursivas en DNS.

-- Consulta iterativa

Definición y propósito
Es un método de resolución DNS que permite buscar información gradualmente.
Distribuye la carga entre múltiples servidores para mejorar el rendimiento y la fiabilidad.
Proceso básico
El resolver comienza consultando servidores de nombres raíces.
Continúa con servidores autorizados del dominio superior.
Finaliza en servidores específicos del dominio objetivo.
Beneficios clave
Mejora la escalabilidad y reducción de latencia.
Aumenta la tolerancia a fallos al permitir alternativas rápidas.
Configuración
La mayoría de resoladores modernos lo realizan por defecto.
Requiere configuración adecuada en los servidores DNS.
Este resumen captura las ideas más esenciales sobre la consulta iterativa DNS, enfocándose en su definición, proceso básico y beneficios principales.