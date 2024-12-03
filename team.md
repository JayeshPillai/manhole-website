---
title: Team
permalink: /team
layout: collection
collection: people
entries_layout: grid

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

flexgallery3:
  - aspect: "3.25"
    image_path: /assets/img/mvrimages/animation_placeholder.png
    alt: "Animation Film Placeholder"
    title: "Animation Film Placeholder"

---
<div class="tab-buttons">
  <button id="vr-team" class="tab-button active">VR Team</button>
  <button id="animation-film" class="tab-button">Animation Film</button>
</div>

<div id="content-vr-team" class="tab-content active">
  
  # **Collaborators**

  This project is a collaboration between award-winning animators, VR filmmakers, and experienced developers and artists.

  {% include flexgallery id="flexgallery2" caption="" %}

  ## **Supported by**
  <div style="width:100%; max-width:200px; margin-top: 0px">
    <a href="https://www.unrealengine.com/" target="_blank">
      <img src="{{ site.url }}{{ site.baseurl }}/assets/img/mvrimages/unreal.png" alt="">
    </a>
  </div> 
  <br>
  <small style="color:grey"><i>The short film was supported by Epic Games.</i></small><br>

  Manhole Collective invites collaborations and contributions by all who wish to participate in initiating social change on the issues connected to manual scavenging. [Reach out to us.](/contact)
</div>

<div id="content-animation-film" class="tab-content">
  
  # **Animation Film**

  The animation film explores a deeply engaging narrative that highlights critical social issues. Stay tuned for more updates about our animation efforts.

  {% include flexgallery id="flexgallery3" caption="" %}
</div>

<style>
.tab-buttons {
  display: flex;
  gap: 10px;
  margin-bottom: 20px;
}

.tab-button {
  padding: 10px 20px;
  border: none;
  border-radius: 20px;
  font-size: 16px;
  cursor: pointer;
  background-color: #f9ece9;
  color: #e67c7c;
  font-weight: bold;
  transition: all 0.3s ease;
}

.tab-button.active {
  background-color: #e67c7c;
  color: white;
}

.tab-button:hover {
  background-color: #e67c7c;
  color: white;
}

.tab-content {
  display: none;
}

.tab-content.active {
  display: block;
}

hr {
  height: 1px;
  border-width: 0;
  color: #fcd5ce;
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
});
</script>
