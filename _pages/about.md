---
layout: about
title: About
permalink: /


news: true  # includes a list of news items
latest_posts: true  # includes a list of the newest posts
selected_papers: false # includes a list of papers marked as "selected={true}"
social: true  # includes social icons at the bottom of the page
---


<div class="row">
    <div class="Slideshow" style="margin-bottom:1cm;">
        <img class="mySlides" src="/assets/img/BannerPhotos/240119_LabPhotoCrop.JPG" style="width:100%;border-radius:5px;">
        <img class="mySlides" src="/assets/img/BannerPhotos/STORM B sub cell wall crop.png" style="width:100%;border-radius:5px;">
        <img class="mySlides" src="/assets/img/BannerPhotos/ExcitationModuleCrop.png" style="width:100%;border-radius:5px;">
    </div>
</div>


Welcome to the Holden Lab website! 

We are interdisciplinary scientists who study bacterial cell biology and biophysics using super-resolution microscopy and other advanced imaging methods. Our primary biological focus is how bacteria remodel their cell wall, which is one of the most important targets​ for antibiotics. 

We are based in the <a href="https://warwick.ac.uk/services/estates/news/ibrb_opening/">Interdisciplinary Biosciences Research Building</a>, in the 
<a href="https://warwick.ac.uk/fac/sci/lifesci/">School of Life Sciences</a>, University of Warwick, near Coventry, UK. 


Key research themes:

- Mechanistic principles of bacterial cell wall remodelling
- Single molecule & super-resolution microscopy
- Open source scientific software and hardware

<script>
    var myIndex = 0;
    carousel();

    function carousel() {
        var i;
        var x = document.getElementsByClassName("mySlides");
        for (i = 0; i < x.length; i++) {
            x[i].style.display = "none";  
        }
        myIndex++;
        if (myIndex > x.length) {myIndex = 1}    
        x[myIndex-1].style.display = "block";  
        setTimeout(carousel, 4000); // Change image every 2 seconds
    }
</script>