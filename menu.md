---
title: Menu
layout: default
permalink: /menu/

---

<div class="card card-nav-tabs card-plain">
                <div class="card-header card-header-danger">
                  <!-- colors: "header-primary", "header-info", "header-success", "header-warning", "header-danger" -->
                  <div class="nav-tabs-navigation">
                    <div class="nav-tabs-wrapper">
                      <ul class="nav nav-tabs" data-tabs="tabs">
                        <li class="nav-item">
                          <a class="nav-link active show" href="#all" data-toggle="tab">All</a>
                        </li>
                        <li class="nav-item">
                          <a class="nav-link" href="#snacks" data-toggle="tab">Snacks</a>
                        </li>
                        <li class="nav-item">
                          <a class="nav-link" href="#drinks" data-toggle="tab">Drinks</a>
                        </li>
                      </ul>
                    </div>
                  </div>
                </div>
                <div class="card-body ">
                  <div class="tab-content text-center">
                    <div class="tab-pane active show" id="all">
                    {% assign sorted_snacks = site.churro_cafe | sort: "category" %}
                        <div class="churros">
                            {% for churro in sorted_snacks %}
                              <div class="churro">
                                  <h5>{{ churro.title }}</h5>
                                  {{ churro.content }}
                                  <a href="{{ churro.url }}">Eat</a>
                              </div>
                            {% endfor %}
                        </div>
                    </div>

                    <div class="tab-pane" id="snacks">          
                      {% assign sorted_snacks = site.churro_cafe | sort: "category" %}
                      <div class="churros">
                          {% for churro in sorted_snacks %}
                              {% if churro.categories contains 'snacks' %}
                                <div class="churro">
                                    <h5>{{ churro.title }}</h5>
                                    {{ churro.content }}
                                </div>
                              {% endif %}  
                          {% endfor %}
                        </div>
                    </div>

                    <div class="tab-pane" id="drinks">
                    {% assign sorted_snacks = site.churro_cafe | sort: "category" %}
                    <div class="churros">
                        {% for churro in sorted_snacks %}
                            {% if churro.categories contains 'drinks' %}
                              <div class="churro">
                                    <h5>{{ churro.title }}</h5>
                                    {{ churro.content }}
                              </div>
                            {% endif %}  
                        {% endfor %}
                    </div>                      

                    </div>
                  </div>
                </div>
              </div>
