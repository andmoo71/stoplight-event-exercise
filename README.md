// (function() {
  'use strict';

  //GREEN BUTTON CONTROL

  const goButton = document.getElementById("goButton");
  const goLight = document.getElementById("goLight");

  function turnGreen(event) {

    if (goLight.className === `bulb`) {
      goLight.className = `bulb go`;
    } else if (goLight.className === `bulb go`) {
      goLight.className = `bulb`;
    };//if stat.
    
  };//func.

  goButton.addEventListener("click", turnGreen);

  //--------------------------------------------------
  //YELLOW BUTTON CONTROL

  const slowButton = document.getElementById("slowButton");
  const slowLight = document.getElementById("slowLight");
  
  function turnYellow(event) {
    
    if (slowLight.className === 'bulb') {
      slowLight.className = `bulb slow`;
    } else if (slowLight.className === `bulb slow`) {
      slowLight.className = `bulb`
    };//if stat.

  };

  slowButton.addEventListener("click", turnYellow);
  
  //--------------------------------------------------
  //RED BUTTON CONTROL
  const stopButton = document.getElementById("stopButton");
  const stopLight = document.getElementById("stopLight");
  
  function turnRed(event) {
    
    if (stopLight.className === 'bulb') {
      stopLight.className = `bulb stop`;
    } else if (stopLight.className === `bulb stop`) {
      stopLight.className = `bulb`
    };//if stat.

  };
  
  stopButton.addEventListener("click", turnRed);

  //--------------------------------------------------

  function enterStop(event) {
    console.log(`Entered Stop button`);
  };

  stopButton.addEventListener(`mouseover`, enterStop);

  function leftStop(event) {
    console.log(`Left Stop button`);
  };

  stopButton.addEventListener(`mouseleave`, leftStop);

 //--------------------------------------------------

 function enterSlow(event) {
  console.log(`Entered Slow button`);
 };

 slowButton.addEventListener(`mouseover`, enterSlow);

 function leftSlow(event) {
  console.log(`Left Slow button`);
 }

 slowButton.addEventListener(`mouseleave`, leftSlow);

 //--------------------------------------------------



  //--------------------------------------------------






  
  // YOUR CODE HERE
// })();
