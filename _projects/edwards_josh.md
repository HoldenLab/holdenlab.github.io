---
layout: page
title: Josh Edwards
description: PhD student
img: assets/img/people/josh_edwards_profile.jpg
importance: 201
category: current
redirect: 
---

<div class="page">
    <div class="row">
        <div class="col">
            <h4>About Me</h4>
            <hr>
            <p>I studied for an MPhys in physics at the Univeristy of Kent from 2015-2019. During this time I completed two internships in the <a href="https://micronoxford.com/">Micron Bioimaging facility</a> at Oxford Univeristy developing python code to asses abberations in adaptive optics systems and to identify regions of interest in biological samples using machine learining. For my masters project I joined Kent's <a href="https://research.kent.ac.uk/applied-optics/">Applied Optics Group</a> where I worked on a remote focusing infra-red <a href="https://www.nature.com/articles/s43586-022-00162-2">optical coherence microscope</a> for the optical biopsy of skin cancers.</p>
            <p>During my PhD I have developed advanced microscopes including leading the <a href="https://holdenlab.github.io/LifeHackWebsite">LifeHack microscope</a> project.</p>
            <p>I have a strong passion for open science and so all of my work is available through the LifeHack microscope website and the Holden Lab <a href="https://github.com/HoldenLab">GitHub</a></p>
        </div>
        <div class="col">
            <img src="/assets/img/people/josh_edwards_profile.jpg" width="100%" style="border-radius:5px;">
        </div>
    </div>
    <h4>My Projects</h4>
    <hr>
    <h5>LifeHack Microscope</h5>
    <p>The LifeHack microscope is an open-source microscopy project capable of SMLM and live cell imaging surpassing existing commercial systems. It is intended to be equally useful as designed or as a development platform from which to build specialised systems to solve cutting edge problems.</p>
    <video src="/assets/img/Video/Microscope-Full-animation.mp4" id="LH_animation" width="90%" style="margin-bottom:1cm;border-radius:5px;" controls autoplay muted></video>
    <p>The microscope is constructed from commercially available and 3D printed parts to simplify the build process and comprehensive parts lists, CAD files, and build/setup instructions are available through a <a href="https://holdenlab.github.io/LifeHackWebsite">custom website</a> to allow straightforward construction of the microscope.</p>
    <h5>ImLock Sample Stabilisation</h5>
    <p>ImLock is an infra-red, image based, 3D microscope drift correction tool. It operates as a micromanager plugin and with minimal additional hardware making it addible to any system. Using a hybrid live/post-hoc correction technique I have been able to achieve long term sample stability of <b>~5nm</b> in Z and <b>~2nm</b> in X and Y.</p>
    <p>The code is available on GitHub <a href="https://github.com/HoldenLab/DeepAutoFocus/releases">here</a> and detailed documentation can be found <a href="https://holdenlab.github.io/LifeHackWebsite/ImageAutofocus.html">here</a>.</p>

</div>

<script>

    var videoEl = document.getElementById("LH_animation");
    var videoWasStarted = false;

    window.addEventListener('scroll', function(e) {
        if (isScrolledIntoView(videoEl) && !videoWasStarted) {
            videoWasStarted = true;
            videoEl.play();
        }
    });

    function isScrolledIntoView(el) {
        var elemTop = el.getBoundingClientRect().top;
        var elemBottom = el.getBoundingClientRect().bottom;

        var isVisible = (elemTop >= 0);
        return isVisible;
    }

</script>