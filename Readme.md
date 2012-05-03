# Accelerando

The Accelerando web service assists users (primarily singers and teachers of singing) in building vocal recital and concert programs. One to 1½ hours in length, a vocal recital or concert program consists of 4-6 sets of pieces. These sets may be composed of a single cycle of pieces or a group of individual pieces that aren’t part of a composer-created cycle. Sets usually focus on one topic such as a composer, a character, a time period, a geographic location, or a theme.

Data in the Accelerando web service is split into a list resource of cycles, a list resource of pieces, resources of individual cycles, and resources of individual pieces. Note that in our service "piece" exists at a conceptually higher level than a particular edition of printed music. That is, a "piece" in the Accelerando web service is analogous to a "work" in the FRBR model rather than an expression. Users will be able to search for pieces and cycles of music that are appropriate for the voice category of the singer in order ultimately to compose an aesthetically pleasing voice recital or concert program.

## Attribute values: name, id, class, rel

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

### Extend existing type to make it more specific. 

We extended the existing type CreativeWork to the narrower type MusicComposition [itemtype="http://schema.org/CreativeWork/MusicComposition"], which inherits all the properties of CreativeWork as well as defining new properties specific to MusicComposition. New properties of MusicComposition are documented below:
    itemprop="opusNumber"
    itemprop="numberWiOpus"
    itemprop="alternateLanguage"
    itemprop="textSource"
    itemprop="instrumentation"
    itemprop="key"
    itemprop="altKey"
    itemprop="tempo"
    itemprop="metMark"
    itemprop="range"
    itemprop="tessitura"
    itemprop="difficulty"

We extended the Person type to a narrower type Character [itemtype="http://schema.org/Person/Character"], which inherits all the properties of Person as well as defining new properties specific to Character. New properties of Character are documented below:
    itemprop="ageRange"
    itemprop="socialStatus"

### Extend existing property to make it more specific.

We extended the existing creator property of CreativeWork for composers and poets. Extensions of existing properties are documented below:
    itemprop="creator/composer"
    itemprop="creator/poet"

### Use properties from non-Schema.org vocabularies.

We used two properties from non-Schema.org vocabularies:
    itemprop="http://purl.org/dc/terms/isPartOf"
    itemprop="http://purl.org/dc/terms/relation"

## Ideas to implement in later versions of Accelerando

### Use JavaScript to dynamically add new text input fields on demand (say, when the user clicked an "Add New Subject" button).

### Implement a reconciliation service that, given an ambiguous identifier such as "Bach", would suggest unambiguous identifiers such as possble Library of Congress identifiers.

### Use JavaScript to convert inputted MIDI numbers to letter numbers for display such as "Middle C".

### Use HTML to dynamically change allowable values for MIDI numbers associated with notes.