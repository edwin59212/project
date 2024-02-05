Project on digitalclock using html,css and javascript =Approach
Create the webpage structure in HTML using a div tag containing dummy time of time format “HH:MM:SS”.
Style the page with CSS using elements and classes defined in HTML.
In JavaScript define a function showTime and render it every second using JavaScript setInterval() method.
Create a new instance of time using JavaScript new Date().
Convert it into string format and show the output
function showTime() {
    // Getting current time and date
    let time = new Date();
    let hour = time.getHours();
    let min = time.getMinutes();
    let sec = time.getSeconds();
    am_pm = "AM";
 
    // Setting time for 12 Hrs format
    if (hour >= 12) {
        if (hour > 12) hour -= 12;
        am_pm = "PM";
    } else if (hour == 0) {
        hr = 12;
        am_pm = "AM";
    }
 
    hour =
        hour < 10 ? "0" + hour : hour;
    min = min < 10 ? "0" + min : min;
    sec = sec < 10 ? "0" + sec : sec;
 
    let currentTime =
        hour +
        ":" +
        min +
        ":" +
        sec +
        am_pm;
 
    // Displaying the time
    document.getElementById(
        "clock"
    ).innerHTML = currentTime;
}
 
showTime();
MULTIPLACTION APP
Functions are the building blocks of some specific code that carry out specific tasks. Using the function, we can multiply two numbers by passing parameters, and the function will then return the result of the multiplication.
