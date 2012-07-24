# Calendar Picker

This is a scrollable Calendar Picker largly based on the work done by Roberto Bicchierai ([link](http://roberto.open-lab.com/2010/04/06/ultra-light-jquery-calendar/)) .

[DEMO](http://d2burke.com/exp/scroll-date-picker/)

**The CSS used in the demo was designed for Google Chrome, visual results may vary based on the browser you use.


## Usage

1. Download and unpack
2. Link to the jquery.calendarPicker.js and jquery.calendarPicker.css files
3. Create a <div> element in your 
4. Attach the calendarPicker method to your newly created div by its id after the all of the other elements in your HTML, or in a doc ready function in the head

    <script>
        $(document).ready(function(){
            var calendarPicker1 = $("#picker1").calendarPicker({
                monthNames:["Jan", "Feb", "Mar", "Apr", "May", "Jun", "Jul", "Aug", "Sep", "Oct", "Nov", "Dec"],
                dayNames: ["Sun", "Mon", "Tue", "Wed", "Thu", "Fri", "Sat"],
                showDayArrows:false,
                vertical: true,
                callback:function(cal) {
					$("#display").html("Selected date: " + cal.currentDate);
                }
            });
        });

    </script>

    <body>

    
    <div id="calendar"></div>

    </body>
	

## Change Log

### 0.1.0

* First release
* Add this CI project to any existing CI project
* Run setup to create supporting database schema


## Donations

Developed by Daniel Burke, [D2 Development](http://www.d2burke.com)