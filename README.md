# Spotify | Carto Resources

Spotify | Carto Resources

Musical Cities Map:
[https://github.com/spotifymaps/spotifymaps.github.com/tree/master/musicalcities](https://github.com/spotifymaps/spotifymaps.github.com/tree/master/musicalcities)

Future Maps Template:
[https://github.com/spotifymaps/spotifymaps.github.com/tree/master/maptemplate](https://github.com/spotifymaps/spotifymaps.github.com/tree/master/maptemplate)

### Spotify | Carto Basemap URL:
	http://cartobase-{s}.global.ssl.fastly.net/spotify_dark/{z}/{x}/{y}.png?api_key=es5j1lspt00gaafhlaw0qa4mrijx61nm0bgnnhah

### iframe embed code example

	https://embed.spotify.com/?uri=spotify:user:thesoundsofspotify:playlist:01s3zfdCTwJ8yaeX5sbS7J&theme=white&width=285&height=360&frameborder=0&allowtransparency=true


To Reproduce the Spotify | Carto Map Template:

1. Get the `viz.json` from your map viz. Get it from here (copy that orange highlighted link): 

<img src="img/publish.png"  style="width:75%;">

2. Put it here: 

<img src="img/put_vizjson_here.png"  style="width:75%;">

### infoWindow Example for Cities


<img src="img/infowindows_for_cities.png"  style="width:75%;">

	<style>
	
	  @font-face{font-family:Circular;src:url('https://sp-bootstrap.global.ssl.fastly.net/7.3.0/fonts/circular-book.woff2') format('woff2'),url('https://sp-bootstrap.global.ssl.fastly.net/7.3.0/fonts/circular-book.woff') format('woff');font-weight:400;font-style:normal}
	
	  @font-face{font-family:Circular;src:url('https://sp-bootstrap.global.ssl.fastly.net/7.3.0/fonts/circular-medium.woff2') format('woff2'),url('https://sp-bootstrap.global.ssl.fastly.net/7.3.0/fonts/circular-medium.woff') format('woff');font-weight:500;font-style:normal}
	
	  @font-face{font-family:Circular;src:url('https://sp-bootstrap.global.ssl.fastly.net/7.3.0/fonts/circular-bold.woff2') format('woff2'),url('https://sp-bootstrap.global.ssl.fastly.net/7.3.0/fonts/circular-bold.woff') format('woff');font-weight:700;font-style:normal}  
	  
	</style>  
	  
	  <div class="cartodb-popup v2">
	  <a href="#close" class="cartodb-popup-close-button close">x</a>
	  <div class="cartodb-popup-content-wrapper">
	    <div class="cartodb-popup-content">
	      <!--<h4>description</h4>-->      
	<img src="https://dl.dropboxusercontent.com/u/36281098/images/spotify_small.png" width="100%">
	      <img src="{{name}}" width="20%" align="right">
	      <p style='font-size: 18px; font-family: "Circular", sans-serif; font-weight: 700; padding-bottom: 0px !important'><strong>{{city}}</strong></p>
	       <p>
	      <iframe src="{{link}}" theme="white" width="280" height="360" frameborder="0" allowtransparency="true"></iframe></p>
	
	    </div>
	  </div>
	  <div class="cartodb-popup-tip-container"></div>
	</div>
	
### infoWindow example for Countries


<img src="img/infowindow_code.png"  style="width:75%;">


	<style>
	
	  @font-face{font-family:Circular;src:url('https://sp-bootstrap.global.ssl.fastly.net/7.3.0/fonts/circular-book.woff2') format('woff2'),url('https://sp-bootstrap.global.ssl.fastly.net/7.3.0/fonts/circular-book.woff') format('woff');font-weight:400;font-style:normal}
	
	  @font-face{font-family:Circular;src:url('https://sp-bootstrap.global.ssl.fastly.net/7.3.0/fonts/circular-medium.woff2') format('woff2'),url('https://sp-bootstrap.global.ssl.fastly.net/7.3.0/fonts/circular-medium.woff') format('woff');font-weight:500;font-style:normal}
	
	  @font-face{font-family:Circular;src:url('https://sp-bootstrap.global.ssl.fastly.net/7.3.0/fonts/circular-bold.woff2') format('woff2'),url('https://sp-bootstrap.global.ssl.fastly.net/7.3.0/fonts/circular-bold.woff') format('woff');font-weight:700;font-style:normal}
	  
	div.cartodb-popup .jspContainer{
	  height: 500px !important;
	  }
	  
	</style>  
	  
	  <div class="cartodb-popup v2" style="height:525px; !important">
	  <a href="#close" class="cartodb-popup-close-button close">x</a>
	  <div class="cartodb-popup-content-wrapper">
	    <div class="cartodb-popup-content">
	      <p style='font-size: 18px; color: #fff; font-family: "Circular", sans-serif; font-weight: 700; padding-bottom: 0px !important'><strong>{{geounit}}</strong></p>
	      <!--<h4>description</h4>-->      
	<!--<img src="https://dl.dropboxusercontent.com/u/36281098/images/spotify_small.png" width="100%">--> 
	      <!--<img src="{{name}}" width="20%" align="right">-->
	      <!--<p style='font-size: 18px; font-family: "Circular", sans-serif; font-weight: 700; padding-bottom: 0px !important'><strong>{{country}}</strong></p>-->
	       <!--<p>-->
	      <p style='font-size: 12px; font-family: "Circular", sans-serif; font-weight: 700; padding-bottom: 0px !important; padding-top: 10px;'><strong> Distinctive</strong></p>
	      <p><!--Distinctive-->
				<iframe src="https://embed.spotify.com/?uri={{distinctiv}}&theme=white" theme="white" width="270" height="80" frameborder="0" allowtransparency="true"></iframe></p>
	      <p style='font-size: 12px; font-family: "Circular", sans-serif; font-weight: 700; padding-bottom: 0px !important; padding-top: 10px;'><strong>Emerging</strong></p>
	      <p><!--Emerging-->
	      <iframe src="https://embed.spotify.com/?uri={{emerging_t}}&theme=white" theme="white" width="270" height="80" frameborder="0" allowtransparency="true"></iframe></p>
	      <p style='font-size: 12px; font-family: "Circular", sans-serif; font-weight: 700; padding-bottom: 0px !important; padding-top: 10px;'><strong>Most Popular</strong></p>
	      <p><!--Most Popular-->
	      <iframe src="https://embed.spotify.com/?uri={{most_popul}}&theme=white" theme="white"  width="270" height="80" frameborder="0" allowtransparency="true"></iframe></p>
	      <p style='font-size: 12px; font-family: "Circular", sans-serif; font-weight: 700; padding-bottom: 0px !important; padding-top: 10px;'><strong>Most Viral</strong></p>
	      <p><!--{{country}}-->
	      <iframe src="https://embed.spotify.com/?uri={{most_viral}}&theme=white" theme="white" width="270" height="80" frameborder="0" allowtransparency="true"></iframe></p>  
	    </div>
	  </div>
	  <div class="cartodb-popup-tip-container"></div>
	</div>	
	
	