### Lab 1, Beginner Track

1. On GitHub, fork the <a href="https://github.com/codefellows/F2-JavaScript-lab1-beg-track">lab 1 repo</a> by clicking the "fork" button in the upper right.
2. On your version of the repo, copy the "HTTPS clone url", midway down the right-hand side of your repo. It should be something like this: https://github.com/yourusernamehere/lab1-beg-track.git
3. Open your terminal and navigate to your projects directory.
4. Run this: `git clone thelinkyoujustcopiedgoeshere`
5. Change directories into your lab folder: `cd lab1-beg-track`
6. Run `npm install`.
7. Your assignment is in lab1.js. There are detailed instructions in the
comments. Be sure to read everything. Run lab.js with `node lab1.js`.
8. Before you turn in your assignment, run `grunt` to check for jshint and jscs errors/warnings. Fix all the errors.
9. List any resources you used (blogs, stack overflow questions, etc.) or collaborators below.


#### Resources and Collaborators

MDN / W3School:
- return
- Math.random()
- Math.floor()
- split()
- join()
- array methods (push, pop, shift, unshift, splice)
- closures (related to return statements)


Stackoverflow:
- replace item in array with javascript
- grunt install issues


#### Clare's Meerkat problem solution for comparison:

var sentence1 = 'More food please.';
var splitString = sentence1.split(" ");
for (var i=0; i< splitString.length; i++){
  splitString[i]= "chirp";
}
sentence1 = splitString.join([separator = ' '])



var sentence2 = 'Come over here so you can scratch my belly.';
var splitString2 = sentence2.split(' ');
var j = splitString2.length;
while (j--){
  splitString2[j] = "chirp";
};
sentence2 = splitString2.join([separator = ' '])


#### Alex's Meerkat problem solution for comparison:

var sentence1 = 'More food please.';
var sentence2 = 'Come over here so you can scratch my belly.';

function meerkatSpeak(words) {
  words = words.split(" ");
  for (var i = 0; i < words.length; i++) {
    words[i] = "chirp";
  }
  words = words.join(" ") + ".";
  return words;
}

console.log(meerkatSpeak(sentence1));
console.log(meerkatSpeak(sentence2));
