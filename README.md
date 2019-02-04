# Movistargazzing

No es nada nuevo el hecho que Netflix se toma muy enserio la seguridad de su RED y la proteccion de su contenido DRM con fin de evitar a toda costa la reproduccion ilegal de su contenido propietario.  

Lo que si es nuevo es la oferta de NETFLIX ilimitado atravez dela red movistar. La red movistar es una red MNO compuesta de un numero de redes MVNE, MVNO osease que no le pertenece toda la infraestructura de red mobil con la cual provee estos servicios.

Sabiendo esto; seria possible redirigir mi traffico local atravez de sockets con fin de routear todas los pedidos de mi cel ala red de distribucion de contenido de netflix (CDN) atravez de la red movistar ?????

# implementacion:

Tunnel SSH con instancias SSL 



#netmap

What port does Netflix device streaming use?  Ihe service uses HTTP and HTTPS session protocols (SSL-443) to netflix's CDN. 

Security requirements, control mechanisms, and general architecture
Netflix concerns, from a security point of view, are:

Only users with the correct (unlimited) plan can access content
Users don’t share their account information with others
Videos are only accessible from within the US, due to licensing restrictions
Video content cannot be redistributed and played at a later time
Those restrictions are enforced by a set of coordinated mechanisms:

- Request user authentication before playing the video
- Allow a maximum of six playback devices (browsers, Roku, etc.) per account
- Reject requests that come from IP addresses outside of the US range
- Encrypt the video content
- Provide unique decryption keys per movie and device


