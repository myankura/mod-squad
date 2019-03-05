original code:

//const HTMLRepresentation = `<h1>The Mod Squad</h1>`//should go here

{
    const ModSquad = {
    
        //add a , between members array and series.//
        
        "members": ["Pete Cochran", "Linc Hayes", "Julie Barnes", "Capt. Adam Greer", "Chief Barney Metcalf"]
        "series": {
            "start": "1968",
            "end": "1973"
        }
    }
    //move scope up outside of opening { //
    const HTMLRepresentation = `<h1>The Mod Squad</h1>`

    ModSquad.members.forEach(member => {
        //remove const
        const HTMLRepresentation += `<div>${member}</div>`
    })
}

//add += in between inner.html and HTMLRepresentation
document.querySelector(".show-info").innerHTML = HTMLRepresentation
