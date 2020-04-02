---
title: Menu
layout: default
permalink: /menu/

---
{% for churro in site.churro_cafe %}
{{ churro.title }}
{{ churro.content }}
{% endfor %}
<div class="card card-nav-tabs card-plain">
                <div class="card-header card-header-dark">
                  <!-- colors: "header-primary", "header-info", "header-success", "header-warning", "header-danger" -->
                  <div class="nav-tabs-navigation">
                    <div class="nav-tabs-wrapper">
                      <ul class="nav nav-tabs" data-tabs="tabs">
                        <li class="nav-item">
                          <a class="nav-link" href="#home" data-toggle="tab">All</a>
                        </li>
                        <li class="nav-item">
                          <a class="nav-link" href="#updates" data-toggle="tab">Snacks<div class="ripple-container"></div></a>
                        </li>
                        <li class="nav-item">
                          <a class="nav-link active show" href="#history" data-toggle="tab">Drinks<div class="ripple-container"></div></a>
                        </li>
                      </ul>
                    </div>
                  </div>
                </div>
                <div class="card-body ">
                  <div class="tab-content text-center">
                    <div class="tab-pane" id="home">
                        {% for churro in site.churro_cafe %}
                    </div>
                    <div class="tab-pane" id="updates">

                    </div>
                    <div class="tab-pane active show" id="history">

                    </div>
                  </div>
                </div>
              </div>
