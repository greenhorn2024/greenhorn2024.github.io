+++
title = 'About'
date = 2024-01-12T16:12:04+01:00
draft = false
+++

<h2 id="countdown"></h2>

<script>
// Set the date we're counting down to
var countDownDate = new Date("Aug 1, 2024 00:00:00").getTime();

// Update the count down every 1 second
var x = setInterval(function() {

  // Get today's date and time
  var now = new Date().getTime();

  // Find the distance between now and the count down date
  var distance = countDownDate - now;

  // Time calculations for days, hours, minutes and seconds
  var days = Math.floor(distance / (1000 * 60 * 60 * 24));
  var hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
  var minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
  var seconds = Math.floor((distance % (1000 * 60)) / 1000);

  // Display the result in the element with id="demo"
  document.getElementById("countdown").innerHTML = "Deadline in " + days + "d " + hours + "h "
  + minutes + "m " + seconds + "s ";

  // If the count down is finished, write some text
  if (distance < 0) {
    clearInterval(x);
    document.getElementById("countdown").innerHTML = "Deadline for applications is over!";
  }
}, 1000);
</script>

The Greenhorn meeting is a conference held annually, which targets junior researchers (those who are within the first-half
of PhD or in the last year of their masters) working in the research areas of *quantum optics*, *nano optics*, *atomic physics* and
*ultra-cold atomic gases* so that they share their knowledge and exchange ideas. The aim, in addition to providing an
opportunity to give a talk and present a poster, is to provide a platform for connecting and networking among junior
researchers in their respective fields of research.
