-------- Creating Constructor Functions ----------------

function BellBoy (name, age, hasWorkPermit, languages) {
    this.name = name;
    this.age = age;
    this.hasWorkPermit = hasWorkPermit;
    this.languages = languages;
    this.moveSuitcase = function () {
        alert ("May I take your suitcase?");
        pickUpSuitCase ();
        move ();
    }
}

var bellboy1 = new BellBoy("Timmy", 19, true, ["French, "English"]);
-----------------------------------------------------------

---------------- Objects and Methods ----------------------
var houseKeeper1 = {

    name: "Hamon",
    age: 27,
    yearsOfExperience: 4,
    languages: ["english", "french"]
    moveSuitcase: function () {
        alert ("May I take your suitcase?");
        pickUpSuitCase ();
        move ();
    }
}; 

houseKeeper1.moveSuitcase();
-------------------------------------------------------------

------- CallsBacks and Listening to Events ------------------
Higher order functions: functions that are able to take functions as inputs (functionception)
Callback function: waits for something to finish happening before executing
Ex:
    document.addEventListener("keypress", respondToKey(event));

    function respondToKey(event){
        console.log("Key pressed.");
    }
Ex2:
    function anotherEventListener(typeOfEvent, callback) {
        //Detect Event Code
    var eventThatHappened = {
        eventType: "keypress",
        durationOfKeyPress: 2;
    }

    if (eventThatHappened.eventType === typeOfEvent) {
        callback(eventThatHappened)
    }
    }