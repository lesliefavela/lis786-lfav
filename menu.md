---
title: Menu
layout: default
permalink: /menu/

---

<div class="card card-nav-tabs card-plain">
                <div class="card-header card-header-success" style="width:600px;">
                  <!-- colors: "header-primary", "header-info", "header-success", "header-warning", "header-danger" -->
                  <div class="nav-tabs-navigation">
                    <div class="nav-tabs-wrapper">
                      <ul class="nav nav-tabs" data-tabs="tabs">
                        <li class="nav-item active">
                          <a class="nav-link active" href="#all" data-toggle="tab">All</a>
                        </li>
                        <li class="nav-item">
                          <a class="nav-link" href="#snacks" data-toggle="tab">Snacks<div class="ripple-container"></div></a>
                        </li>
                        <li class="nav-item">
                          <a class="nav-link" href="#drinks" data-toggle="tab">Drinks<div class="ripple-container"></div></a>
                        </li>
                      </ul>
                    </div>
                  </div>
                </div>
                <div class="card-body ">
                  <div class="tab-content text-center">
                    <div class="tab-pane" id="all">
                    {% for churro in site.churro_cafe %}
                    {{ churro.title }}
                    {{ churro.content }}
                    {% endfor %}
                    </div>
                    <div class="tab-pane" id="snacks">

                    </div>
                    <div class="tab-pane active show" id="drinks">

                    </div>
                  </div>
                </div>
              </div>
