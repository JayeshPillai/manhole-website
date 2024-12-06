---
title: Team
permalink: /team
layout: collection
collection: people
entries_layout: grid

flexgallery3:
  - aspect: "3.25"
    url: https://imxd.in/
    image_path: /assets/img/mvrimages/partners_logo_imxdlab.png
    alt: "IMXD Lab"
    title: "IMXD Lab"
  - aspect: "3.25"
    url: http://www.idc.iitb.ac.in/
    image_path: /assets/img/mvrimages/partners_logo_idc.png
    alt: "IDC School of Design, IIT Bombay"
    title: "IDC School of Design, IIT Bombay"
  - aspect: "3.25"
    url: https://opod.in/
    image_path: /assets/img/mvrimages/partners_logo_opod.png
    alt: "Opod Films & Media"
    title: "Opod Films & Media"
  - aspect: "3.25"
    url: https://www.deckor.co/
    image_path: /assets/img/mvrimages/partners_logo_deckor.png
    alt: "Deckor.co"
    title: "Deckor.co"    
  - aspect: "3.25"
    url: /contact
    image_path: /assets/img/mvrimages/partners_logo_seekmy.png
    alt: "Seekmy Technology"
    title: "Seekmy Technology"

flexgallery2:
  - aspect: "3.25"
    url: https://imxd.in/
    image_path: /assets/img/mvrimages/partners_logo_imxdlab.png
    alt: "IMXD Lab"
    title: "IMXD Lab"
  - aspect: "3.25"
    url: http://www.idc.iitb.ac.in/
    image_path: /assets/img/mvrimages/partners_logo_idc.png
    alt: "IDC School of Design, IIT Bombay"
    title: "IDC School of Design, IIT Bombay"
  - aspect: "3.25"
    url: https://www.deckor.co/
    image_path: /assets/img/mvrimages/partners_logo_deckor.png
    alt: "Deckor.co"
    title: "Deckor.co"
    

---

<div class="tab-buttons">
  <button id="vr-narrative" class="tab-button active">VR Narrative</button>
  <button id="animation-film" class="tab-button">Animation Film</button>
</div>

<div id="content-vr-narrative" class="tab-content active">
  <h3>Collaborators</h3>
  <p>
    This project is a collaboration between award-winning animators, VR filmmakers, and experienced developers 
and artists.
  </p>
  {% include flexgallery id="flexgallery2" caption="" %}

  <h3>Supported by</h3>
  <div style="width:100%; max-width:80px; margin-top: 0px">
    <a href="https://www.iitb.ac.in/" target="_blank">
      <img src="{{ site.url }}{{ site.baseurl }}/assets/img/mvrimages/iitb_png.png" alt="IIT Bombay">
    </a>
  </div>

<small style="color:grey"><i>The production of  the VR Narrative was supported by IRCC, IIT Bombay</i></small>
  <br><br>
  <p>
    Manhole Collective invites collaborations and contributions by all who wish to participate in initiating social change 
on the issues connected to manual scavenging.
  </p>

</div>


  <br>


<div id="content-animation-film" class="tab-content">
  <h3>Collaborators</h3>
  <p>
    This project is a collaboration between award-winning animators, VR filmmakers, and experienced developers and artists.
  </p>
  {% include flexgallery id="flexgallery3" caption="" %}

  <h3>Supported by</h3>
  <div style="width:100%; max-width:200px; margin-top: 0px">
    <a href="https://www.unrealengine.com/" target="_blank">
      <img src="{{ site.url }}{{ site.baseurl }}/assets/img/mvrimages/unreal.png" alt="Unreal Engine">
    </a>
  </div>
  <br>
  <small style="color:grey"><i>The short film was supported by Epic Games.</i></small>
  <br><br>
  <p>
    Manhole Collective invites collaborations and contributions by all who wish to participate in initiating social change on the issues connected to manual scavenging. 
    <a href="{{ site.baseurl }}/contact" target="_self">Reach out to us.</a>
  </p>
</div>

<style>

.tab-buttons {
  display: flex;
  gap: 10px;
  margin: 30px 0;
  border-bottom: 2px solid #F0BF4C;
}

.tab-button {
  padding: 10px 20px;
  border: none;
  border-radius: 5px 5px 0 0;
  font-size: 16px;
  cursor: pointer;
  background-color: #FFE8BB;
  color: #000000;
  font-weight: bold;
  outline: none;
}

.tab-button:focus {
  outline: none;
}

.tab-button.active {
  background-color: #F0BF4C;
  color: black;
}

.tab-button:hover {
  background-color: #F0BF4C;
  color: #000000;
}

.tab-content {
  display: none;
}

.tab-content.active {
  display: block;
}

h3 {
  font-weight: 900; 
  font-size: 1.5em; 
  color: #000000; 
}

hr {
  height: 0;
  border-width: 0;
  color: #000000;
  background-color: #fcd5ce;
}
</style>

<script>
document.addEventListener("DOMContentLoaded", function () {
  const buttons = document.querySelectorAll('.tab-button');
  const contents = document.querySelectorAll('.tab-content');

  buttons.forEach(button => {
    button.addEventListener('click', () => {
      buttons.forEach(btn => btn.classList.remove('active'));
      contents.forEach(content => content.classList.remove('active'));

      button.classList.add('active');
      document.getElementById(`content-${button.id}`).classList.add('active');
    });
  });

  // Ensure links inside tab content are not blocked
  const links = document.querySelectorAll('.tab-content a');
  links.forEach(link => {
    link.addEventListener('click', function (event) {
      event.stopPropagation(); // Allow the link to work normally
    });
  });
});
</script>
