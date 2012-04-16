Accelerando

====================================

ATTRIBUTE VALUES:

id attribute values:
	id="cycle"
	id="cycleAttributes"
	id="cycleSongs"
	id="piece"
	id="pieceAttributes"
	id="pieceTranspositions"

class attribute values:
	class="idNumber"
	class="composerName"
	class="composerNationality"
	class="poetName"
	class="poetNationality"
	class="Key" 
	class="Range" (notated as MIDI numbers)
	class="instrumentation"
	class="textSource"
	class="language"
	class="genre"
	class="subGenre"
	class="character"
	class="subject"
	class="mood"
	class="tempoMarking" (notated as beats-per-measure)
	class="difficulty"
	class="inclusion"

All Accelerando resources:
	list of all pieces
	list of pieces with a given characteristic
	a single piece
	list of all cycles
	list of all cycles with a given characteristic
	a single song cycle

=========================================

NOTATION:

The URIs for all people (composers and poets) and works (songs, cycles, text sources) will be identified by Library of Congress Subject Heading (LCSH).

LCSH subject heading conversion to URI:
		all punctuation and spaces will be removed 
		all diacritics will be normalized (Ges&auml;nge or Gesänge = Gesaenge)
	examples:
		"Joyce, James, 1882-1941" becomes /JoyceJames18821941/
		"Barber, Samuel, 1910-1981. Nuvoletta" becomes /BarberSamuel19101981Nuvoletta/
		"Brahms, Johannes, 1833-1897. Gesänge, viola, piano acc., op. 91" becomes /BrahmsJohannes18831897Gesaengeviolapianoaccomp91/

The URIs for "range" will be notated in MIDI format (pitches are assigned numbers rather than letter names)
	example: C#'-C''' becomes 61-84

The URIs for "tempo marking" will be notated in beats-per-measure (BPM)
	example: "Andante con moto" becomes 90 BPM

==========================================
	
QUESTIONS/COMMMENTS:

It is possible to create new pieces or cycles. 
How do I specify which cycle a piece belongs to (assuming it does belong to a cycle) within the POST form?

*
RYAN SAYS:
There are various options:
You could have a select list of cycles that the client could select from, or leave unselected for "no cycle."
It could depend on the context; e.g. an "add piece" form on a cycle page could include a hidden "cycle" input that is set to the cycle being currently viewed.
*

Several of the form attributes would be better suited for a non-"text" type. 
I ran out of time to reserach how this would be implemented, but I plan to change this aspect of the forms.


Within the piece and cycle resources, attributes of those pieces/cycles are designated as "class" attributes (exp. <li class="composerName">Composer: <span>Barber, Samuel</span></li>). 
However, within the forms, these same attributes are designated as "name" attributes (exp. <input name="composerName" type="text" />). 
Will this prevent the forms from functioning properly?

*
RYAN SAYS:
No, you've done it correctly.
*

==========================================

RYAN SAYS:

Your attribute values do a good job of describing the data in your representations. 
But you've forgotten to describe the state transitions (links and forms). 
You need to define rel attributes for the links in your application that indicate what kind of resource is being linked to. 
You also need to define class attributes for your forms that indicate what they do.