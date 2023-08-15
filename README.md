# -RandomSentencesGenerator
Thats my first SoftUni Project. It's random sentances genarator.

const readline = require('readline').createInterface ({
    input: process.stdin,
    output: process.studout
})

let names = ['Nikip', 'Mimi', 'Titi', 'Plami', 'Vicki'];
let places = ['Sunny Beach', 'Sozopol', 'Sofia', 'Plovdiv'];
let verbs = ["eats", "holds", "sees", "plays with", "fucks", 'feels'];
let nouns = ['tortilla', 'note', 'phone', 'ID'];
let adverbs = ['slowly', 'sadly', 'diligently'];
let details = ['near the sex shop', 'in the house', 'in the bed'];

function getRandomWord (arr) {
    let word = arr[Math.floor(Math.random()*arr.length)];
    return word;
}

let randomName = getRandomWord(names);
let randomPlace = getRandomWord(places);
let randomVerbs = getRandomWord(verbs);
let randomNouns = getRandomWord(nouns);
let randomAdverbs = getRandomWord(adverbs);
let randomDetails = getRandomWord(details);

let who = `${randomName} from ${randomPlace}`;
let action = `${randomAdverbs} ${randomVerbs} ${randomNouns}`;
let sentance = `${who} ${action} ${randomDetails}`;

console.log(sentance);
