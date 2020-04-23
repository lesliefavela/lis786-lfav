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
                        <li class="nav-item">
                          <a class="nav-link" href="#all" data-toggle="tab">All</a>
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
                        {% for churro in site.churro_cafe %}  
                          <div class="container-fluid content-row">
                              <div class="row">
                                <div class="col-sm-4">
                                  <div class="col-sm-3">
                                    <div class="card m-2" style="width:14rem; height:22rem;">
                                    {{ churro.title }}
                                    {{ churro.content }}
                                      <div class="card-body">
                                        <h5 class="card-title">Champurrado</h5>
                                      </div>
                                    </div>
                                  </div>
                                </div>

                                <div class="col-sm-4">
                                  <div class="col-sm-3">
                                    <div class="card m-2" style="width:14rem; height:22rem;">
                                      <img src="https://www.cookingclassy.com/wp-content/uploads/2019/04/horchata-6.jpg" class="img-card-top" style="height:17rem;">
                                      <div class="card-body">
                                        <h5 class="card-title">Horchata</h5>
                                      </div>
                                    </div>
                                  </div>
                                </div>

                                <div class="col-sm-4">
                                  <div class="col-sm-3">
                                    <div class="card m-2" style="width:14rem; height:22rem;">
                                      <img src="https://d3926qxcw0e1bh.cloudfront.net/post_photos/5a/b7/5ab786ecf1b7b5a0dba379c034a20586.jpeg.max578.jpeg" class="img-card-top" style="height:19rem;">
                                      <div class="card-body">
                                        <h5 class="card-title">Aguas Frescas</h5>
                                      </div>
                                    </div>
                                  </div>
                                </div>
                              </div>
                          </div>
                            {% endfor %}y
                    </div>
                    <div class="tab-pane active show" id="drinks">

                    </div>
                  </div>
                </div>
              </div>
