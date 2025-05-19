+++
title = ""
subtitle = ""
+++

<style>
    header, body, footer 
    {
        font-family: sans-serif;
        color: white;
    }

    html, body 
    {
        margin: 0;
        padding: 0;
        height: 100%;
        background: black;
        overflow: hidden;
        font-family: sans-serif;
    }

    header 
    {
        position: fixed;
        top: 0;
        left: 0;
        width: 100%;
        height: 100px;
        background-color: rgba(0, 0, 0, 0.85);
        display: flex;
        align-items: center;
        justify-content: space-between;
        padding: 0 1rem;
        z-index: 10;
        box-shadow: 0 2px 5px rgba(0, 0, 0, 0.7);
    }

    .logo 
    {
        display: flex;
        align-items: center;
        gap: 0.5rem;
    }

    .logo img 
    {
        height: 64px; /* increase logo image height */
        width: auto;
    }

    .logo span 
    {
        font-size: 2rem; /* increase text size */
        font-weight: bold;
        color: white;
    }

    .video-bg 
    {
        position: fixed;
        top: 56px; /* height of the header */
        left: 0;
        width: 100vw;
        height: calc(100vh - 56px);
        object-fit: cover;
        z-index: 0;
    }

    .page-wrapper 
    {
        position: relative;
        height: calc(100vh - 56px);
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        color: white;
        z-index: 1;
        padding-bottom: 3rem;
        box-sizing: border-box;
    }

    footer 
    {
        position: fixed;
        bottom: 0;
        left: 0;
        width: 100%;
        background: black;
        color: white;
        text-align: center;
        padding: 1rem 0;
        z-index: 2;
    }

    /* Hide Ananke's default header */
    div.pb3-m.pb6-l.bg-black 
    {
        display: none !important;
    }

    header nav a 
    {
        display: inline-block;
        margin-left: 1.5rem;
        color: white !important;
        font-size: 2rem;
        font-family: sans-serif;
        cursor: pointer;
        transition: color 0.2s ease;
        text-decoration: none !important;
    }

    header nav a:hover 
    {
        color: #ccc !important;
        text-decoration: none !important;
    }
</style>

<header>
  <div class="logo">
    <img src="/images/gsops_logo.png" alt="GSOPs Logo">
    <span>CG Nomads</span>
  </div>
  <nav>
    <a href="#about">About</a>
    <a href="#features">Features</a>
    <a href="#contact">Contact</a>
  </nav>
</header>

<video class="video-bg" autoplay loop muted playsinline>
  <source src="/videos/gsops_meshing.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>