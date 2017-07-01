<!DOCTYPE html>
<html>
<head>
      <link href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css" 
            rel="stylesheet" 
            integrity="sha384-BVYiiSIFeK1dGmJRAkycuHAHRg32OmUcww7on3RYdg4Va+PmSTsz/K68vbdEjh4u" 
            crossorigin="anonymous">
      <script src="../salert/dist/sweetalert.min.js"></script>
<link rel="stylesheet" type="text/css" href="../salert/dist/sweetalert.css">
      <!--<link href="../bootstrap/dist/css/bootstrap.css" rel="stylesheet">
      <link href="../bootstrap/dist/css/bootstrap-theme.css" rel="stylesheet">-->
      <script
       src="https://code.jquery.com/jquery-3.2.1.js"
       integrity="sha256-DZAnKJ/6XZ9si04Hgrsxu/8s717jcIzLy3oi35EouyE="
       crossorigin="anonymous"></script>
       <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js" 
               integrity="sha384-Tc5IQib027qvyjSMfHjOMaLkfuWVxZxUPnCJA7l2mCWNIpG9mGCD8wGNIcPD7Txa"
               crossorigin="anonymous"></script>
      <!-- <link href="../bootstrap/dist/js/bootstrap.js" rel="stylesheet">-->
      <link href="page1.css" rel="stylesheet">
      <script src="myscript.js"> </script>  
 <link rel="shortcut icon" type="image/x-icon" href="../images/notebg.png" />
<title>
Project-Meir Landau 
</title>
</head>


<body onload="loadTasks()">

 <!--- - - - - - - - - - - - - - - - - -          Title      - - - - - - - - - - - - - - - - -->
    
    <div class="title">
    <img src="../images/title.png"> 
    </div>
    
<!---       - - - - - - - - - - - - - -     First container     - - - - - - - - - - - - - - - -->


     <div class="container">
        <div class="first">
              <input type="text" title="NAME (ex: David Dupont)" class="form-control" id="usr" placeholder="Tape your name here !">
        </div>
        <div class="second">
              <input type="text" title="Your Task (ex: Homework)"class="form-control" id="desc" placeholder="What you don't have to forget!">
        </div>
        <div class="third"id="third">
           
        </div>
        <div class="for">
            <label > Date : </label>  <input type="date" id="date" value="Date" > 
            <label >Hour :  </label><input type="time" id="txthour" value="hour"> 
        </div>
        <div class=five>
                <button type="button" 
                        id="btn" 
                        onclick="addTask($('usr').value,$('desc').value,$('date').value,$('txthour').value)" 
                        class="btn btn-success" >Send</button>
        </div>
    </div>
    <ul id="myTaskList">
          
    </ul>

</body>
</html>
