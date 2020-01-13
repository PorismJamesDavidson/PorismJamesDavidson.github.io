---
Title: Title
---

<a href="/page/">Test</a>
<div id="readme"></div>
{% include README.md %}  
<script src="https://code.jquery.com/jquery-3.4.1.min.js" crossorigin="anonymous"></script>   
<script src="https://cdnjs.cloudflare.com/ajax/libs/showdown/1.9.1/showdown.js" integrity="sha256-44/UcMYgn8vlo2B5ydHmUcy9SXMt7bg2RhftDR35kY8=" crossorigin="anonymous"></script> 
<div id="docs"></div>
<script>  
  $(function() {
      $.get( "https://raw.githack.com/esd-org-uk/human-services/master/Schemas/documentation.html", function( data ) {
        $( "#docs" ).html( data );
      });      
      $.get( "https://rawcdn.githack.com/esd-org-uk/human-services/909f9161bdfda3cab3448c2ed09faa18a974ae90/README.md", function( data ) {
        let convert = new showdown.Converter();
        $( "#readme" ).html(convert.makeHTML(data));
      });
  });
  
</script>  