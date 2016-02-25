# JavaScript-code
// JavaScript Document



//This is the first function. It converts Warchest Points to C-Bills
function myFunction() {
      var y = document.getElementById("warcps").value;
	  	
		//This if statement will report an error is letters are used
	  	if (isNaN(y)) 
  			{
   				//alert("Must input numbers");
    			document.getElementById("cbs").innerHTML = "You must input only numbers!"
				return false;
  			}
	  
      var x = +y * 34904;
      document.getElementById("cbs").innerHTML = x.toLocaleString();
      			}
				
//This is the second function. It converts C-Bills into Warchest Points.				
function myFunction2() {
      var a = document.getElementById("cb").value;
	  	
		//This if statement will report an error is letters are used
		if (isNaN(a)) 
  			{
   				document.getElementById("wps").innerHTML = "You must input only numbers!";
    			return false;
  			}
	 
	  var b = +a / 34904;
     //Since Warchest Points can't be used in increments of less than 1, the reported WPs are rounded up to the next number at 0.5.
	  document.getElementById("wps").innerHTML = Math.round(b).toLocaleString();
      			}

//This function clears all data on the page.
function resetPage() {
    location.reload();
}


 
