---
title: Menu
layout: default
permalink: /menu/

---
{% for churro in site.churro_cafe %}
{{ churro.title }}
{{ churro.content }}
{{% endfor %}}
<div class="card card-nav-tabs card-plain">
                <div class="card-header card-header-danger">
                  <!-- colors: "header-primary", "header-info", "header-success", "header-warning", "header-danger" -->
                  <div class="nav-tabs-navigation">
                    <div class="nav-tabs-wrapper">
                      <ul class="nav nav-tabs" data-tabs="tabs">
                        <li class="nav-item">
                          <a class="nav-link" href="#home" data-toggle="tab">Home</a>
                        </li>
                        <li class="nav-item">
                          <a class="nav-link" href="#updates" data-toggle="tab">Updates<div class="ripple-container"></div></a>
                        </li>
                        <li class="nav-item">
                          <a class="nav-link active show" href="#history" data-toggle="tab">History<div class="ripple-container"></div></a>
                        </li>
                      </ul>
                    </div>
                  </div>
                </div>
                <div class="card-body ">
                  <div class="tab-content text-center">
                    <div class="tab-pane" id="home">
                      <p>I think that’s a responsibility that I have, to push possibilities, to show people, this is the level that things could be at. So when you get something that has the name Kanye West on it, it’s supposed to be pushing the furthest possibilities. I will be the leader of a company that ends up being worth billions of dollars, because I got the answers. I understand culture. I am the nucleus.</p>
                    </div>
                    <div class="tab-pane" id="updates">
                      <p> I will be the leader of a company that ends up being worth billions of dollars, because I got the answers. I understand culture. I am the nucleus. I think that’s a responsibility that I have, to push possibilities, to show people, this is the level that things could be at. I think that’s a responsibility that I have, to push possibilities, to show people, this is the level that things could be at. </p>
                    </div>
                    <div class="tab-pane active show" id="history">
                      <p> I think that’s a responsibility that I have, to push possibilities, to show people, this is the level that things could be at. I will be the leader of a company that ends up being worth billions of dollars, because I got the answers. I understand culture. I am the nucleus. I think that’s a responsibility that I have, to push possibilities, to show people, this is the level that things could be at.</p>
                    </div>
                  </div>
                </div>
              </div>
