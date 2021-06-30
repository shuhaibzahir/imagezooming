# imagezooming
this is simple image zooming
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    
    main image
   
    <div class="main-image-wapper">
     <img class=" imageView" src="image source data-large="/image source" alt="">
   </div>
  
 
  
                                                                                
              one function for image gallery
                                                                                
               $(document).on('click','your thumbnailClass',function(){
                var url = $(this).data('url'); //put there data-url with image source
           
               $(this).closest('this is main div').find('tagName').each(function(){
               $(this).removeClass('active');
               })
               $(this).addClass('active');
               $(this).closest('.this is main div').find('yourBigsize image class').attr('src',url);
               $(this).closest('.this is main div').find('.yourBigsize image class').attr('data-large',url);
               return false;
        })
                                                                                
 

                                                                                
                                                                                
  <script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.4.0/jquery.min.js"></script>
<script src="/zoom/zoomsl.js"></script>                                                                       
                                                                                
                                                                                
                                                                                
   
                             
                             if youw want glass style add this
  <style>
      .glass{
          border-radius: 100px;
          border: 5px solid #fff;
      }
  </style>
  
     
                             this is main code 
                             
                             
 <script>
        $(document).ready(function () {
            $(".imageView").imagezoomsl({
   
        if you wabt more option add this
                          
               innerzoommagnifier: true,
                classmagnifier: "glass",
                magnifiersize: [200, 200],
                disablewheel: false  //
    
            });
        });
    </script>
  
</body>
</html>
