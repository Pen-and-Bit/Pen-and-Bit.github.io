
<!DOCTYPE html>
  <head>
    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <title> Main Page </title>
    <meta name="description" content="">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link rel="stylesheet" href="site.css">
    <!-- Latest compiled and minified CSS -->
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.5.0/css/bootstrap.min.css">

    <!-- jQuery library -->
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>

    <!-- Popper JS -->
    <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.16.0/umd/popper.min.js"></script>

    <!-- Latest compiled JavaScript -->
    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.5.0/js/bootstrap.min.js"></script>
    
  </head>
  <body> 
    <div class="text-center bg-dark title-header">
      <header class="display-1 text-light"> Pen and Bit</header>
      <h1 class="text-secondary"> Writing on writing and other topics.</h1>
    </div>

    <button class="tablink" onclick="openPage('Home', this, '#3a2820')" id="defaultOpen">Home</button>
    <button class="tablink" onclick="openPage('Writing', this, '#3a2820')">Writing</button>
    <button class="tablink" onclick="openPage('Design', this, '#3a2820')">Design</button>
    <button class="tablink" onclick="openPage('Software', this, '#3a2820')">Software</button>
    
    <div id="Home" class="tabcontent">
      <h3>1</h3>
      <p>1.</p>
    </div>

    <div id="Writing" class="tabcontent">
      <h3>2</h3>
      <p>2</p>
    </div>

    <div id="Design" class="tabcontent">
      <h3>3</h3>
      <p>3</p>
    </div>

    <div id="Software" class="tabcontent">
      <h3>4</h3>
      <p>4</p>
    </div>





    <script>
      function openPage(pageName,elmnt,color) {
        var i, tabcontent, tablinks;
        tabcontent = document.getElementsByClassName("tabcontent");
        for (i = 0; i < tabcontent.length; i++) {
          tabcontent[i].style.display = "none";
        }
        tablinks = document.getElementsByClassName("tablink");
        for (i = 0; i < tablinks.length; i++) {
          tablinks[i].style.backgroundColor = "";
        }
        document.getElementById(pageName).style.display = "block";
        elmnt.style.backgroundColor = color;
      }
      
      // Get the element with id="defaultOpen" and click on it
      document.getElementById("defaultOpen").click();
      </script>

  </body>
</html>