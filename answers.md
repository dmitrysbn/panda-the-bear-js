# Part 1

# Question 1a
var image = document.querySelector('img');
image.src = "https://patiliyo.com/wp-content/uploads/2017/07/ruyada-kedi-gormek.jpg";

# Question 1b
var image = document.getElementsByClassName("photography")[0];
image.src = "https://placebear.com/325/225";

# Question 2
var heading = document.querySelector('h1.highlight');
heading.innerText = "Dmitry Serbin";

# Question 3
var heading = document.querySelector('div#employment h3.info-title');
heading.innerText = "EMPLOYMENT";

# Question 4
var body = document.querySelector('body');
body.style.color = "red";

# Question 5
var highlights = document.querySelectorAll('.highlight');
highlights.forEach(function(element) {
  element.style.color = "white";
  });

# Question 6
var h1s = document.querySelectorAll('h1');
h1s.forEach(function(e) {
  e.style.fontFamily = 'monospace';
  });

# Question 7
var roundIcons = document.querySelectorAll('a.action-icon-bg');
roundIcons.forEach(function(e) {
  e.style.backgroundColor = "red";
  });

# Question 8
var nameField = document.querySelector('#name');
nameField.placeholder = "Identify yourself";

# Question 9
var messageField = document.querySelector('#message');
messageField.placeholder = "State your business";

# Question 10
nameField.value = "your nemesis";

# Question 11
var emailField = document.querySelector('#email');
emailField.value = "koalathebear@gmail.com";

# Question 12
var submitButton = document.querySelector('#submit');
submitButton.value = 'En garde!';

# Question 13
submitButton.disabled = true;

# Question 14
var aside = document.querySelector('aside.highlight');
var bioInfo = document.querySelector('.bio-info');
aside.removeChild(bioInfo);


# Part 2

# Question 1a
var timeTravel = document.querySelector('#time-travel').parentNode;
document.querySelector('body section div').removeChild(timeTravel);

# Question 1b
var pikachuDrawing = document.querySelector('#right-image');
var portfolioContainer = document.querySelector('.portfolio-container');
portfolioContainer.appendChild(pikachuDrawing.cloneNode(true));

# Question 2
for (var i = 0; i < 10; i++) {
  portfolioContainer.appendChild(pikachuDrawing.cloneNode(true));
}

# Question 3
var listItem = document.createElement('li');
listItem.classList.add('bio-info-item');

var leftSpan = document.createElement('span');
var lastUpdated = document.createTextNode('Page last updated on');
leftSpan.appendChild(lastUpdated);
leftSpan.classList.add('bio-info-title');
listItem.appendChild(leftSpan);

var rightSpan = document.createElement('span');
var date = new Date();
var lastUpdatedText = document.createTextNode(date);
rightSpan.appendChild(lastUpdatedText);
rightSpan.classList.add('bio-info-value', 'bio-info-last-updated');
listItem.appendChild(rightSpan);

var unorderedList = document.querySelector('ul.bio-info');
unorderedList.appendChild(listItem);
