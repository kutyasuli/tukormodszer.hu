---
layout: default
title: Nyitólap
underMenu: Home
frontpage: true
---

<header>
<div class="jumbotron" style="background-image: url('images/banner.jpg'); background-repeat: repeat">
  <div class="container">
    <div style="height: 10px"></div>
    <h1 style="color: #014872; font-size: 48px">Tükör Módszer</h1>
    <p style="color: #014872; font-size: 20px"><i>
      „Nem az a cél, hogy minden kutyát egységesen tökéletesre neveljünk, hanem hogy mi emberek tudatosan alakítsuk ki kapcsolatunkat kutyánkkal és értsük meg őt, hogy mi miért történik.”</i>
    </p>
  </div>
</div>
</header>


<div class="container">
  <div class="row">

      <div class="col-md-6">
        <h3>Ön a Tükör módszert kereste, ha..</h3>       
        <ul style="padding-left: 15px">
          <li> fontos Önnek, hogy kutyája kiegyensúlyozott, egészséges, szófogadó legyen</li>
          <li> szeretné megérteni kutyája viselkedését, igényeit, hogy mit miért csinál</li>
          <li> szeretné kutyáját más kutyák között is elengedni úgy, hogy ne kelljen aggódnia és ő játszhasson kedvére</li>
          <li> nem a kutyát okolja a problémákért, hanem elfogadja, hogy a kutya viselkedése a gazdin múlik</li>
          <li> nem szeretné kedvencét kényszerrel (pórázon rángatva, fenekét lenyomva) tanítani</li>
          <li> az alapvető feladatokon túl mást is megtanítana a kutyájának úgy, hogy közben mindketten jól érezzék magukat</li>
          <li> szeret kutyájával közös, tartalmas programokon részt venni</li>
          <li> szereti kutyáját és felelős állattartónak vallja magát</li>
        </ul>
        Nézzen szét oldalunkon, ismerje meg a módszerünket és keresse meg az Önhöz legközelebb lévő Tükör iskolát!
      </div>


      <div class="col-md-6">
        <h3>Cikkek</h3>
        <!-- counter is a hack, see http://stackoverflow.com/questions/13568052/filter-or-group-a-collection-in-liquid -->
        {% assign counter = '' %}
        {% for post in site.posts %}
          {% if post.category == "cikk" and counter.size < 5 %}
            <a href="{{ post.url }}">{{ post.title }}</a> <small>({{ post.date | date: "%Y.%m.%d." }})</small><br/>
            {% capture counter %}{{ counter | append:'.' }}{% endcapture %}
          {% endif %}
        {% endfor %}
        <br>
        <a href="/cikkek">Minden cikk...</a>
     </div>

  </div>

</div>
