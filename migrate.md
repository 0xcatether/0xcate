<html lang="en">
  <head>
    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1, user-scalable=no">
    <meta name="description" content="">
    <meta name="author" content="">
    <link rel="icon" href="images/favicon.ico">
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css" integrity="sha384-Gn5384xqQ1aoWXA+058RXPxPg6fy4IWvTNh0E263XmFcJlSAwiGgFAW/dAiS6JXm" crossorigin="anonymous">	  
</head>

<body class="">

<div class="container" style="width: 650px;">
  <div class="row">
	<div class="col-lg-12">
		<h1 class="text-center">0xCATE token migration</h1>
		<hr/>
		<br/>
	</div>
	<div id="loader">
	  <p class="text-center">Loading...</p>
	</div>
	<div id="content"  style="display: none;">
	  <p>
		<!--Old token balance <input type="text" class="old-token-balance"></input>-->
		Old token balance
	  </p>
	  <span class="old-token-balance"></span>
	  <br/>
	  <p>
		New token balance
	  </p>	  
		  <span class="new-token-balance"></span>
	  <br/>
	  <form onSubmit="App.migrateTokens(); return false;" role="form">
		<div class="form-group">
		  <div class="input-group">
			<span class="input-group-btn">
			  <button type="submit" class="btn btn-primary btn-lg">Migrate tokens</button>
			</span>
		  </div>
		</div>
	  </form>
	  <br>
	  <hr>
	  <p id="accountAddress"></p>
	  <br>
	  <p class="last-tx-info" hidden>View last transaction on Etherscan: <a class="last-tx-link" href="" target="_blank"></a></p>
	  <br>
	</div>
  </div>
</div>
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/1.12.4/jquery.min.js"></script>
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/js/bootstrap.min.js" integrity="sha384-JZR6Spejh4U02d8jOt6vLEHfe/JQGiRRSQQxSfFWpi1MquVdAyjUar5+76PVCmYl" crossorigin="anonymous"></script>
   <script src="app.js"></script>
</body>
</html>
