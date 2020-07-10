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
	<div id="content" class="text-center" style="display: none;">
	  <p>
		<!--Old token balance <input type="text" class="old-token-balance"></input>-->
		Old token balance <span class="old-token-balance"></span>
	  </p>
	  <br/>
	  <p>
		New token balance <span class="new-token-balance"></span>
	  </p>
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
<!-- ./wrapper -->
  	
	<!-- jQuery (necessary for Bootstrap's JavaScript plugins) -->
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/1.12.4/jquery.min.js"></script>
    <!-- Include all compiled plugins (below), or include individual files as needed -->
    <script src="css/bootstrap.min.js"></script>
    <!--<script src="vendor/truffle-contract/dist/truffle-contract.js"></script>-->
    <script src="app.js"></script>

