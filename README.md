# CORS-Headers-from-Ads.txt-file---preflight---PHP-
The ads.txt file contains verified domains which are referenced before allowing a CORS header response.

<h2>Problem:</h2>
<p>Websites that host advertising are sometimes asked to place an "ads.txt" file in the root of their website. The ads.txt file contains domains where the advertisment will originate from and several other comma separated fields. Not much information is available about the Cross-Origin Resource Sharing (<a href="https://developer.mozilla.org/en-US/docs/Web/HTTP/Guides/CORS" title="Mozilla CORS Reference Guide">CORS</a>) permissions that the advertisors will require between your website and your end-user's browser. 
  <br> The most common and <b>undesirable</b> guidance is to add a wild-card ( 'Access-Control-Allow-Origin' '*' ) to your configuration allowing basic CORS permissions to any source (Origin) domain.  
</p>
Google AdSense Help (<a href="https://support.google.com/adsense/answer/12171612" title="ads.txt help">ads.txt</a>)<br>
IAB Tech Lab (<a href="https://iabtechlab.com/wp-content/uploads/2019/03/IAB-OpenRTB-Ads.txt-Public-Spec-1.0.2.pdf" title="ads.txt ver 1.0.2">ads.txt Specification Version 1.0.2 (pdf)</a>)<br>

<h2>Concept:</h2>
<h5><i>Can we query the the local ads.txt file, prepare a list of allowed-domains and then answer CORS requests on a dynamic per-page basis?</i></h5>
<p>The most obvious language for this would be PHP, and an outfit called <a href="https://wpsandbox.net/development/send-cors-headers-php-p909" title="CORS code tutorial">WPsandbox.net</a> has a PHP example for how to make the dynamic responses.</p>

<a href="https://www.juannicolas.eu/how-to-set-up-nginx-cors-multiple-origins/">NGINX example</a><br>
<a href="https://ubiq.co/tech-blog/set-access-control-allow-origin-cors-headers-apache/">APACHE example</a><br>


