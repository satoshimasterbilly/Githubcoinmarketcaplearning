<script type = "text/javascript">

// split the urls to make it manageable
 let BASE_URL = "https://api.coingecko.com/api/v3/";
 let ENDPOINT = "coins/markets?vs_currency=usd&order=market_cap_desc&per_page=100&page=1&sparkline=true&price_change_percentage=24h";
 let GLOBAL = "global";

 //concatenate the urls
 let url = BASE_URL + ENDPOINT;

 fetch(url).then(response => {

   response.json().then(data => {

    console.log(data);

    $.each(data,function(index, value){
    	// console.log(value.market_cap_rank)
    	// document.write("Coin="+value.name)

      $("#data").append("<tr><td>"+value.symbol+"</td><td><img src='"+value.image+"' width='40'></td><td>"+value.name+"</td><td>"+value.market_cap+"</td><td>"+value.current_price+"</td><td>"+value.total_volume+"</td><td>"+value.circulating_supply+"</td><td>"+value.price_change_percentage_24h+"</td><td>"+value.last_updated+"</td></tr>")

        })
    })
  })


  var counter = 10;
var myFunction = function() {
    counter *= 10;
    setTimeout(myFunction, counter);
}
setTimeout(myFunction, counter);
    </script>
  </body>
</html>
