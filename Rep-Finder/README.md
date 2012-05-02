# Accelerando

The Accelerando web service assists users (primarily singers and teachers of singing) in building vocal recital and concert programs. One to 1½ hours in length, a vocal recital or concert program consists of 4-6 sets of pieces. These sets may be composed of a single cycle of pieces or a group of individual pieces that aren’t part of a composer-created cycle. Sets usually focus on one topic such as a composer, a character, a time period, a geographic location, or a theme.

Data in the Accelerando web service is split into a list resource of cycles, a list resource of pieces, resources of individual cycles, and resources of individual pieces. Users will be able to search for pieces and cycles of music that are appropriate for the voice category of the singer in order ultimately to compose an aesthetically pleasing voice recital or concert program.

## Attribute values: id, class, rel

Notes from Ryan: Your attribute values do a good job of describing the data in your representations. 
But you've forgotten to describe the state transitions (links and forms). 
You need to define rel attributes for the links in your application that indicate what kind of resource is being linked to. 
You also need to define class attributes for your forms that indicate what they do.

### id attribute values:
	id="cycle"
	id="cycleAttributes"
	id="cycleSongs"
	id="piece"
	id="pieceAttributes"
	id="pieceTranspositions"

### class attribute values:
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

### rel attribute values:

## Accelerando resources
	list of all pieces
	list of pieces with a given characteristic
	a single piece
	list of all cycles
	list of all cycles with a given characteristic
	a single song cycle

## PUT vs. POST (how URIs are assigned to resources, which create/update forms are located in which resources)

## Extending schema.org

### MusicalComposition, a proposed narrower type of CreativeWork

### Character, a proposed narrower type of Person

### Extending existing properties of CreativeWork

### Using non-schema.org vocabularies

=========================================

The URIs for "range" will be notated in MIDI format (pitches are assigned numbers rather than letter names)
	example: C#'-C''' becomes 61-84

The URIs for "tempo marking" will be notated in beats-per-measure (BPM)
	example: "Andante con moto" becomes 90 BPM