# SolarPCB-BUG-
Full project with schematic, board and datasheets of the solar consumption board

In deze repo zit alles wat ik heb gebruikt voor mijn pcb. De schema's van ieder develop bordje en mijn eigen pcb.
Ook telkens de datasheet van mijn gebruikte IC's

## -BUG-

het probleem waar ik mee zit.
Als ik het systeem laat werken, zonder dat ik er een batterij op aansluit, is het stabiel en blijft het werken.
Vanaf ik er een batterij op aansluit, dan valt na 2 a 3 min de stroom weg en valt de laadspanning van 4,2V --> 2,7V.

De laadstroom die ik kan meten gedurdende de 2 a 3 werkende minuten is 3,7 a 3,9 mA met een laadspanning van 4,2V.

Als ik de PCB eens los maak van de zonnepanneel en terug aansluit, dan werkt de PCB terug voor enkele minuten en valt daarna terug uit.
Ook als ik de capaciteit ontlaadt, werkt het terug, maar dan kom ik gewoon terug in de start postitie te staan, waardoor het logisch is dat hij terug werkt.

Het is IC MCP73871 die uitvalt. Op zijn uitgang (Vbat) komt er dan een spanning van 2.7V en in werkende toestand staat daar een spanning van 4,2V, alle IC's erna, zijn afhankelijk van deze IC, dus de MCP73871 kan maximaal 2.7V meer leveren aan de batterij, wat te weinig is.

Eerst dacht ik dat de ingangsspanning te hoog was voor de IC, waardoor hij uitschakelde, of sneuvelde omdat mijn zonnepanneel 7V leverde en er max 6V op de ingang van de IC mocht komen. Ik heb er een 7805 tussen geplaatst, maar tevergeefs.

mochten er nog zaken niet duidelijk zijn over het probleem, mag je mij altijd een mailtje sturen, of op teams een DM sturen.

Alvast bedankt!

Tom Van Hove
