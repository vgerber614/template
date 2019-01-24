---
layout: essay
type: essay
title: The Bad Question Virus
# All dates must be YYYY-MM-DD format!
date: 2019-01-23
labels:
  - Questions
  - Answers
  - StackOverflow
---

## Bad Questions... They Exist...

<img  align="right" src="../images/goodvsbad.jpg">

Many might say bad questions simply do not exist, but I think they do, we have just been restricting the idea of what can be bad about a question. I would argue that having a question can never be "bad" or "stupid"; however, the way you word it can be "bad". I like to think of bad questions as a virus that infects others with questions. A poorly presented question can leave others confused, leading to more questions spreading. This makes it harder to get quick, clear, and concise answers because the conversation is infected with this bad question disease that it has to get through first. Sometimes, these questions don't get answered at all. Often times, people will completely flock away from the man with the bad question virus, ignoring it to refrain from getting into its mess.

## Asking Smarter, Takes You Farther!

A good question is one that is detailed yet to the point. All the information needed to answer the question is given and nothing else. Providing too much unnecessary details can overwhelm the answerer and possibly even cause further confusion. When you ask someone a question, you want to make sure you bring them up to the same page, without making them read every single page before. This is the most efficent and effective way to get good answers.

## Asking On StackOverflow

<img class="ui small center image" src="../images/stackoverflow_comic.png">

<img align="left" width="100" height="100" src="../images/stackoverflow_icon.png">

Stack Overflow, a question and answer site for programmers, is a great resource for anyone who may have issues with code or who may simply want to learn new or different methods of doing something. There I found examples of good questions and bad questions, which could probably be improved.

In the following example, we examine the components of a decent question. In this case, the asker is trying to figure out a way to get the date of the previous month in Python.

```
Q: Change an HTML5 input's placeholder color with CSS

Chrome supports the placeholder attribute on input[type=text] elements (others probably do too).

But the following CSS doesn't do anything to the placeholder's value:

Like this:

input[placeholder], [placeholder], *[placeholder] {
    color: red !important;
}
<input type="text" placeholder="Value">

Value will still remain grey instead of red.

Is there a way to change the color of the placeholder text?

```
The asker received 33 responses to his/her question with over 3700 upvotes. The questions is concise yet describes the situation and provides code relevant in demonstrating what is in question. The asker also provided an appropriate title that lets users know what exactly is being discussed in this post. I think one of the reasons why this particular post was able to gather so much attention, was because it has a concise yet revealing title, generalized enough to describe the problem as a question universal to the programming language itself. It is not personal nor vague, thus, people are able to search and want to click on this.

Now, I told you good questions would get good answers. This remains true in this case. This post got many well voted answers, with top accepted answer being extremely detailed and informative!

To see the top answer and more from this question:
https://stackoverflow.com/questions/2610497/change-an-html5-inputs-placeholder-color-with-css?page=1&tab=votes#tab-top

## StackFlow Dont's

While the question above got an impressive amount of upvotes and comments, many get little to none. Often this is reflective of a poorly constructed, "bad" question.

```
Q: javascript image loading issue

Ok basically im an idiot and i dont know what im doing.. i'm a complete javascript noob. All i want is to create a canvas in which it loads an add image, mouth image, a clock image(based on the time) and a pill ON TOP of the clock. I'm using YAIL in this code but i've tried so many ways and im utterly clueless as to what im doing wrong.. Could someone please help me. The pill is also supposed to be eventually be dragged into the mouth and register this on a database. Also i began coding in line out of prove simplicity but when i tried to change it to another file, knowing my luck, it didnt work for god knows what reason.

<!DOCTYPE html>
<html>
<head>
<style> body{ background:#ddd;}
canvas { background:#fff;
 display: block;
 margin: 10px auto; 
 box-shadow: 0 5px 15px #aaa;}</style>
 <script type="text/javascript" src="yail.1.4.js"></script>
 <script type="text/javascript" src="action.js"></script>
</head>
<body>
<canvas id="mycanvas"></canvas>
<script>
var Canvas = function(canvasEl, width, height){
this.el= canvasEl;
this.el.width = width;
this.el.height = height;
this.ctx = canvasEl.getContext("2d");
}
var canvas = new Canvas(document.querySelector("#mycanvas"), 1100, 650);
drawadd();
function drawadd(){
var add = new Image();

add.onload = function() {
    canvas.ctx.drawImage(this, 500,-215);
};
add.src="add.png";
}


drawmouth();
function drawmouth(){
var mouth = new Image();

mouth.onload = function() {
    canvas.ctx.drawImage(this, 100,300,175,100);
};
mouth.src="mouth.png";
}

var currentdate = new Date();
var datetime = currentdate.getHours();
var loader = new YAIL(done, progress, errors);

if(datetime==1||datetime==13){
loader.add("clock/clock1.png");
loader.add("clock/pill.png");
}
else if(datetime==2||datetime==14){
loader.add("clock/clock2.png");
loader.add("clock/pill.png");
}
else if(datetime==3||datetime==15){
loader.add("clock/clock3.png");
loader.add("clock/pill.png");
}
else if(datetime==4||datetime==16){
loader.add("clock/clock4.png");
loader.add("clock/pill.png");
}
else if(datetime==5||datetime==17){
loader.add("clock/clock5.png");
loader.add("clock/pill.png");
}
else if(datetime==6||datetime==18){
loader.add("clock/clock6.png");
loader.add("clock/pill.png");
}
else if(datetime==7||datetime==19){
loader.add("clock/clock7.png");
loader.add("clock/pill.png");
}
else if(datetime==8||datetime==20){
loader.add("clock/clock8.png");
loader.add("clock/pill.png");
}
else if(datetime==9||datetime==21){
loader.add("clock/clock9.png");
loader.add("clock/pill.png");
}
else if(datetime==10||datetime==22){
loader.add("clock/clock10.png");
loader.add("clock/pill.png");
}
else if(datetime==11||datetime==23){
loader.add("clock/clock11.png");
loader.add("clock/pill.png");
}
else if(datetime==0||datetime==12){
loader.add("clock/clock12.png");
loader.add("clock/pill.png");
}


loader.load();
function done(e) { 
    var imageLst = e.images;
    var urlLst = e.urls;
    }
function progress(e) { var current = e.current;
    var total = e.total;
    var image = e.img;
    var pst = current / total * 100; }

function errors(e) { var url = e.url;
    var originalErrorObject = e.error; }

</script>
</body>
</html>

An in depth answer would be greatly appreciated because im such a noob.

```

While the above asker was able to describe their situation in their question, enough where a kind responder was able to provide an accepted answer, it was asked in a way that likely made many turn away from answering. For one, the title does not really describe the problem. "javascript image loading issue" is very vague and likely attracted the attention of those who didn't have that question/solution and remained unseen by people that did. Furthermore, the asker may have provided too much information. The post was lengthy, not to the point. Plus, they provided their entire code despite it not all being relevant to the situation. This surely turned away many potential askers who did not want to sift through the entire problem. 

Fortunately, the asker was able to revieve an answer; however, only one answer. Thus, unlike the previous example, there is not a lot of quality responses in which he/she could choose from. The asker only recieved one upvote, showing its lack of exposure and help to others.

## Conclusion

The trek of Q&A is a two way street. Good answers can come when you work to provide the answerer with a good question. You have to help come up with a solution, by effictively laying out the problem. While taking my deep dive into StackOverflow, I couldn't help but analyze the number of upvotes (or downvotes) on different posts. To me this shows how important it is to create good questions not only to provide yourself with good answers, but to provide others that may have a similar or congruent question to yours. When people upvote, they are letting you know you helped them ask or answer a question to a problem they had themselves. You are ultimately helping other programmers within the community grow and learn by fosturing effective discussion.
