sequenceDiagram

participant browser
participant server

    //The user enters content into input field and presses save.
    on browser side using java script code the new note is added into existing notes list and then page is prompted to be redrawn and after that a post request is sent to server for the new note.
    This way is faster than traditional implementation.
    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
