# Accelerando

The Accelerando web service assists users (primarily singers and teachers of singing) in building vocal recital and concert programs. One to 1½ hours in length, a vocal recital or concert program consists of 4-6 sets of pieces. These sets may be composed of a single cycle of pieces or a group of individual pieces that aren’t part of a composer-created cycle. Sets usually focus on one topic such as a composer, a character, a time period, a geographic location, or a theme.

Data in the Accelerando web service is split into a list resource of cycles, a list resource of pieces, individual cycle resources, and individual piece resources. Note that in our service "piece" exists at a conceptually higher level than a particular edition of printed music. That is, a "piece" in the Accelerando web service is analogous to a "work" in the FRBR model rather than an "expression". Users will be able to search for pieces and cycles of music that are appropriate for the voice category of the singer in order ultimately to compose an aesthetically pleasing voice recital or concert program.

## Attribute values: id, class, rel, and name

### id attribute values:
    create-cycle- Applied to a FORM tag. A form for creating a cycle.
    create-piece- Applied to a FORM tag. A form for creating a piece.
    search-cycle - Applied to a FORM tag. A form for searching across cycles.
    search-piece - Applied to a FORM tag. A form for searching across pieces.
    update-cycle- Applied to a FORM tag. A form for updating a cycle.
    update-piece- Applied to a FORM tag. A form for updating a piece.

### class attribute values:
    admin-forms - Applied to a DIV tag. A set of FORMs for creating and updating. 
    altKey- Applied to a SPAN tag. If the work has been transposed into a different key from the original, this gives the alternative key of the work.
    altLanguage- Applied to a SPAN tag. If the work has been translated, this gives the alternative language of the work.
    characterAgeRange- Applied to a SPAN tag. If the piece is from the point of view of a particular character, this gives the approximate age range of that character.
    characterGender- Applied to a SPAN tag. If the piece is from the point of view of a particular character, this gives the gender of that character.
    characterName- Applied to a SPAN tag. If the piece is from the point of view of a particular character, this gives the name of that character.
    characterSocialStatus- Applied to a SPAN tag. If the piece is from the point of view of a particular character, this gives the social status of that character.
    compDateNum- Applied to a SPAN tag. This gives the composition date of the work in a numerical (HTML date) format.
    compDateText- Applied to a SPAN tag. This gives the composition date of the work in a human readable text format.
    composerName- Applied to a SPAN tag. This gives the name of the composer of the work.
    composerNationality- Applied to a SPAN tag. This gives the nationality of the composer.
    cycleDescription-  Applied to a SPAN tag. This gives the description of the cycle.
    cycleTitle- Applied to a SPAN tag. This gives the title of the cycle.
    difficulty- Applied to a SPAN tag. This gives the difficulty of the piece.
    genre- Applied to a SPAN tag. This gives the genre of the work.
    instrumentation- Applied to a SPAN tag. This gives the instrumentation of the piece.
    list - Applied to a DIV tag. A list of either cycles or pieces.
    listCycles- Applied to a UL tag. A list of cycles. It may have one or more LI.class="oneCycle" descendant elements.
    listPieces - Applied to a UL tag. A list of pieces. It may have one or more LI.class="onePiece" descendant elements.
    metronome- Applied to a SPAN tag. This gives the metronome marking of a piece.
    mood- Applied to a SPAN tag. This gives the mood of the piece.
    numberWiOpus - Applied to a SPAN tag. This gives the number of the piece within its corresponding opus.
    oneCycle - Applied to a LI tag. A single cycle.
    onePiece- Applied to a LI tag. A single piece.
    opusNumber- Applied to a SPAN tag. This gives the opus number of musical composition.
    originalKey- Applied to a SPAN tag. This gives the original key of the piece.
    originalLanguage- Applied to a SPAN tag. This gives the original language of the work.
    pieceDescription - Applied to a SPAN tag. This gives the description of the piece.
    pieceTitle- Applied to a SPAN tag. This gives the title of the piece.
    poetName- Applied to a SPAN tag. This gives the poet of the work.
    poetNationality- Applied to a SPAN tag. This gives the nationality of the poet.
    range- Applied to a SPAN tag. This gives the range of the piece notated as MIDI numbers.
    search - Applied to a DIV tag. A form for searching.
    subject- Applied to a SPAN tag. This gives the subject of the piece.
    tempo- Applied to a SPAN tag. This gives the  tempo of the piece.
    tessitura- Applied to a SPAN tag. This gives the tessitura of the piece.
    textSource- Applied to a SPAN tag. This gives the source for the text of the work.

### rel attribute values:
    cycle- Applied to an A tag. A reference to a cycle page in Accelerando.
    external - Applied to an A tag. A reference to resources external to the Accelerando site.
    index - Applied to an A tag. A reference to the starting URI for the service.
    piece - Applied to an A tag. A reference to a piece page in Accelerando
    stylesheet- Applied to a LINK tag. A link to the CSS stylesheet.


### name attribute values:
    _method - Applied to an INPUT[text] element. Used to specify a non-HTML method (such as PUT).
    item[altKey] - Applied to an INPUT[text] element. An alternative key for the piece.
    item[altLang] - Applied to an INPUT[text] element. An alternative language (e.g. a translation) of the piece.
    item[char] - Applied to an INPUT[text] element. When the piece is in character, the name of the character.
    item[charAgeRange] - Applied to an INPUT[text] element. When the piece is in character, the age range of the character.
    item[charGender] - Applied to an INPUT[text] element. When the piece is in character, the gender of the character.
    item[charSocStat] - Applied to an INPUT[text] element. When the piece is in character, the social status of the character.
    item[comp] - Applied to an INPUT[text] element. The name of the composer.
    item[compDateNum] - Applied to an INPUT[date] element. The composition date of the piece in a numerical date format.
    item[compDateText] - Applied to an INPUT[text] element. A human readable text form of the composition date.
    item[compID] -  Applied to an INPUT[text] element. The Library of Congress authority file for the composer.
    item[compNat] - Applied to an INPUT[text] element. The nationality of the composer.
    item[cycleDescription] - Applied to an TEXTAREA element. A description of the cycle.
    item[cycleID] - Applied to an INPUT[text] element. The Library of Congress authority file for the cycle.
    item[cycleTi] - Applied to an INPUT[text] element. The title of the cycle.
    item[diff] - Applied to an INPUT[text] element. The difficulty of the piece.
    item[genre]- Applied to an INPUT[text] element. The genre of the piece.
    item[imslp] - Applied to an INPUT[text] element. A URI for the IMSLP resources related to the piece.
    item[inst] - Applied to an INPUT[text] element. The instrumentation of the piece.
    item[key] - Applied to an INPUT[text] element. The original key of the piece.
    item[metMark] - Applied to an INPUT[text] element. The metronome marking for the piece.
    item[mood] - Applied to an INPUT[text] element. The mood of the piece.
    item[numberWi] - Applied to an INPUT[number] element. The piece number within the opus.
    item[opusNumber] - Applied to an INPUT[text] element. The opus number.
    item[orgLang] - Applied to an INPUT[text] element. The original language of the piece.
    item[pieceDescription] - Applied to an TEXTAREA element. A description of the piece.
    item[pieceID] - Applied to an INPUT[text] element. The Library of Congress authority file for the piece.
    item[pieceTi] - Applied to an INPUT[text] element. The title for the piece.
    item[poet] - Applied to an INPUT[text] element. The name of the poet.
    item[poetID] -  Applied to an INPUT[text] element. The Library of Congress authority file for the poet.
    item[poetNat] - Applied to an INPUT[text] element. The nationality of the poet. 
    item[range] - Applied to an INPUT[text] element. The range of the piece in terms of MIDI numbers.
    item[subject] - Applied to an INPUT[text] element. The subject of the piece.
    item[subjectID] -  Applied to an INPUT[text] element. The Library of Congress authority file for the subject.
    item[tempo] - Applied to an INPUT[text] element. The tempo of the piece.
    item[tess] - Applied to an INPUT[text] element. The tessitura of the piece.
    item[txtSrc] - Applied to an INPUT[text] element. A source or inspiration for the text of the piece.
    item[worldCat] - Applied to an INPUT[text] element. A URI for a WorldCat query on the title of the piece.

## Accelerando resources
    list of all pieces
    list of pieces with a given characteristic*
    a single piece
    list of all cycles
    list of all cycles with a given characteristic*
    a single cycle
    
    *not yet fully implemented

## PUT vs. POST 
####(how URIs are assigned to resources, which create/update forms are located in which resources)
After some debate, we decided that given the complexity of uniform titles for musical compositions, it would not be worth it to use the uniform title in the URIs. Since no other good way of assigning meaningful URIs would be determined, we decided to use POST for creating both cycles and pieces. PUT is only used for updating pages. 
New cycles are created on the list-cycles page. New pieces are created on the one-cycle page. This allows us to more easily assoicate a piece with a cycle it belongs to. Update forms are on the pages they update.
    
## Extending schema.org

1.  We extended the existing type CreativeWork to the narrower type MusicComposition [itemtype="http://schema.org/CreativeWork/MusicComposition"], which inherits all the properties of CreativeWork as well as defining new properties specific to MusicComposition. We also extended the Person type to a narrower type Character [itemtype="http://schema.org/Person/Character"], which inherits all the properties of Person as well as defining new properties specific to Character.

    #### Properties of new type MusicComposition:
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

    #### Properties of new type Character:
        itemprop="ageRange"
        itemprop="socialStatus"

2. We extended the existing creator property of CreativeWork for composers and poets.

    ####  Extensions of existing properties:
        itemprop="creator/composer"
        itemprop="creator/poet"

3.  We used two properties from non-Schema.org vocabularies.

    #### Dublin Core properties:
        itemprop="http://purl.org/dc/terms/isPartOf"
        itemprop="http://purl.org/dc/terms/relation"

## Ideas to implement in later versions of Accelerando

1. Use JavaScript to dynamically add new text input fields on demand (say, when the user clicked an "Add New Subject" button).

2. Implement a reconciliation service that, given an ambiguous identifier such as "Bach", would suggest unambiguous identifiers such as possble Library of Congress identifiers.

3. Use JavaScript to convert inputted MIDI numbers to letter numbers for display such as "Middle C".

4. Use HTML to dynamically change allowable values for MIDI numbers associated with notes.

5. Create ability to search by more characteristics. 