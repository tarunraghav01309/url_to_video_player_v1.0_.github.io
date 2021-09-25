<!DOCTYPE html>
   <html lang="en">
   <head>
   <title>Url to Video Player-v1.3</title>
   <meta charset="utf-8" />
   <style>
   .center {
   display: flex;
   justify-content: center;
   align-items: center;
   height: 22px;
   border: none; 
   }
   
   .submit_button {
   display: flex;
   justify-content: center;
   height: 23px;
   border: 1px solid #35FFFF; 
   background-color: #FF3333;
   color: white;
   }
   
   .submit_button:active {
   display: flex;
   justify-content: center;
   text-align: center;
   height: 25px;
   border: 3px solid #35FFFF; 
   background-color: #FF3333;
   color: white;
   }
   
   .frame_border{
   display: flex;
   justify-content: center;
   align-items: center;
   height: auto;
   border: 1px solid #35FFFF; 
   }
   
   .input_video_url {
   color: #35FFFF;
   background: #333333;
   border: 1px solid white;
   width:100%;
   }
   
   .input_poster_url {
   color: #35FFFF;
   background: #333333;
   border: 1px solid white;
   width:100%;
   }
   </style>
   </head>
   <body style="background-color: black; color: #FF3333; width: 100%">
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
   <h1 style="text-align: center;">Url to Video Player</h1>
   <p style="text-align: center;">v1.3</p>
   <script>
   window.onload=function(){
   alert('Welcome on "Url to Video Player-v1.3", Please click "OK" to continue!');
   }
   function loadVideo() {
   var vid = document.getElementById('vid3');
   vid.src = document.getElementById('source').value;
   vid.poster = document.getElementById('poster').value;
   }
   </script>
   
   <style type="text/css">
   src {
   margin: 50px auto;
   max-width: 500px;
   }
   </style>
   <div class="frame_border">
   <video id="vid3" controls PictureInPicture width="100%" height="200px" preload="metadata" controlslist="download" autoplay src="">
   </video>
   </div>
   <h1></h1>
   <form action="javascript:loadVideo()">
   Video URL-
   <input class="input_video_url" type="url" id="source" value="" placeholder="Example- http://examplevideosong.mp4"/>
   <p></p>
   Poster URL
   <input class="input_poster_url" type="url" id="poster" value="https://cdn.plyr.io/static/demo/View_From_A_Blue_Moon_Trailer-HD.jpg"/>
   <p></p>
   <div class="center">
   <button class="submit_button" type="submit">Submit</button>
   </div>
   <p></p>
   
   <h1></h1>
   </form>
   </body>
   </html>
