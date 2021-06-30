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
    
  
  
  
  
   <div class="main-image-wapper">
     <img class=" imageView" src="image source data-large="/image source" alt="">
   </div>
  
   {{!-- the image source is very important and you need to add the class name to the down function  and data larg is very important becuase the funtion work with data large --}}
  
                                                                                
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
                                                                                
                                                                                
  {{!--  end  put the code down okay--}} 


                                                                                
                                                                                
  <script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.4.0/jquery.min.js"></script>
<script src="/zoom/zoomsl.js"></script>                                                                       
                                                                                
                                                                                
                                                                                
    //if you want some glass model zoom//
  <style>
      .glass{
          border-radius: 100px;
          border: 5px solid #fff;
      }
  </style>
  
      //if you want some glass model zoom add top code //
 <script>
        $(document).ready(function () {
            $(".imageView").imagezoomsl({
   
   {{!-- (optional) this is for glass else you will get normal --}}
              //  innerzoommagnifier: true,
                classmagnifier: "glass",
                magnifiersize: [200, 200],
                disablewheel: false  //
   
     {{!-- this is for glass else you will get normal  end--}}
   
            });
        });
    </script>
  
</body>
</html>
