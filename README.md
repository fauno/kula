# Kula

## [en]

Kula is an opportunistic file sharing daemon inspired by
[Forban](http://www.foo.be/forban/) but using [Avahi](http://avahi.org)
for peer discovery and [darkhttpd](http://dmr.ath.cx/net/darkhttpd/) for
file serving.

It works like this:

* Start a http server
* And announce itself on the network using DNS-SD
* It'll create a list of shared files on the specified dir.
* Once this happens, it'll search the network for peers
* Download their file list
* Pick a file at random from every peer
* Download the files
* Sleep for a little while
* Update file list and start again...

Eventually every peer will share the same info.  But if you retire early
you'll have new and possibly awesome things!


## [es]

Kula es un compartidor de archivos oportunista inspirado
por [Forban](http://www.foo.be/forban/) pero que usa
[Avahi](http://avahi.org) para el descubrimiento de pares y
[darkhttpd](http://dmr.ath.cx/net/darkhttpd/) para servir los archivos.

Esto es lo que hace:

* Inicia un servidor http
* Y se anuncia en la red local usando DNS-SD
* Crea una lista de archivos compartidos
* Entonces busca pares en la red
* Se descarga su lista de archivos
* Elige un archivo al azar de cada par
* Y los descarga
* Duerme un ratito
* Actualiza la lista y vuelve a empezar...

Eventualmente todos los pares poseen la misma información.  Pero si
te retirás antes vas a terminar con cosas nuevas y posiblemente
geniales!
