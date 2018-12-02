# QMSS

Per lanciare lo script: 

	$ python3 -m main

__N.B__: Eseguire il comando:
	
	$ python3 -m main.py

restituisce questo errore:
	
	/usr/bin/python3: Error while finding module specification for 'main.py'
	(AttributeError: module 'main' has no attribute '__path__')

ovvero, si aspetta che __main__ sia un pacchetto (una cartella contenente moduli) 
invece che un modulo.

Morale della favola: quando ci si riferisce a un modulo, __bisogna sempre omettere
l'estensione .py__, onde evitare bestemmie a profusione.
