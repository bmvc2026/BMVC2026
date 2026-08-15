---
layout: default_sparse
title: Sponsors
permalink: /sponsors/
---

<style>
.sponsor-group {
  margin: 36px 0 48px;
}

.sponsor-group h3 {
  text-align: center;
}

.sponsor-list {
  display: flex;
  flex-wrap: nowrap;
  justify-content: flex-start;
  align-items: center;
  gap: 18px;
  width: max-content;
  max-width: 100%;
  margin: 0 auto;
  overflow-x: auto;
  padding-bottom: 4px;
}

.image-block {
  padding: 14px;
  background: #fff;
  width: 170px;
  height: 150px;
  flex: 0 1 170px;
  min-width: 120px;
  display: flex;
  align-items: center;
  justify-content: center;
  cursor: pointer;
  transition: all .3s ease;
  border: 1px solid transparent;
  box-sizing: border-box;
}

.image-block a {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 100%;
  height: 100%;
}

.image-block img {
  max-height: 120px;
  max-width: 100%;
  object-fit: contain;
}

.image-block:hover {
  border: 1px solid #103a6b;
}
</style>

<p class="mb-3" align="center">We are very grateful to our sponsors for supporting the conference this year.</p>

{% assign sponsor_types = "Platinum+,Platinum,Gold,Silver,Special,Supported by" | split: "," -%}

<section class="sponsors section" align="center">
{% for sponsor_type in sponsor_types %}
    {% assign items = site.data.sponsors.sponsors | where: "type", sponsor_type -%}
    {% if items.size > 0 %}
        <div class="sponsor-group">
            {% if sponsor_type == 'Platinum+' or sponsor_type == 'Platinum' or sponsor_type == 'Gold' or sponsor_type == 'Silver'%} 
                <h3>{{-sponsor_type-}}&nbsp;Sponsors:</h3>
            {% else %}
                <h3>{{-sponsor_type-}}:</h3>
            {% endif %}
            <div class="sponsor-list">
                {% for item in items %}
                    <div class="image-block text-center"{% if item.logo_block_width %} style="width: {{ item.logo_block_width }}; flex-basis: {{ item.logo_block_width }};"{% endif %}>
                        <a href="{{item.url}}" target="_blank" >
                            <img src="{{ site.baseurl }}/imgs_2026/Sponsors/{{ item.logo }}" alt="sponsors-logo" class="img-fluid"{% if item.logo_width %} style="width: {{ item.logo_width }}; max-width: none;"{% endif %}>
                        </a>
                    </div>
                {% endfor %}
            </div>
        </div>
    {% endif %}
{% endfor %}
</section><br>

<div class="align-items-center mb-3">
    <div class="col-xs-12 mx-auto">
        <h2 style="text-align: center;">Sponsoring BMVC</h2>
    </div>
</div>

<div class='text-justify'>
    <!-- <p>If you are interested in sponsoring BMVC 2024, please email <a href="mailto:sponsors@bmvc2024.org">sponsors@bmvc2024.org</a> 
      for more information. The deadline for expressing interest in sponsoring BMVC is <b>30th Septemeber 2024</b>. Thank you so much! -->
    <p>Sponsoring BMVC2026 is the perfect opportunity to showcase your company's excellent work throughout the conference. As a sponsor, you will be provided with a platform to promote your business and work, and numerous opportunities will be available to engage with academic and industrial researchers in the field to explore potential future collaborations. We are open to customising the sponsorship package to best suit your needs.</p>
    <p>If you are interested in sponsoring BMVC 2026, please email <a href="mailto:{{ site.email }}"> {{ site.email }}</a>. The deadline for expressing interest in sponsoring BMVC is <b>28 September 2026</b>.</p>
</div>

<div class="row pl-2 pr-2 pt-2 pb-2 mx-auto justify-content-center">
    <table class="table table-striped table-bordered" style="max-width: 1000px;">
        <tbody>
            <tr>
                <th style="text-align: center">PACKAGE OFFERS</th>
                <th style="text-align: center">PLATINUM+</th>
                <th style="text-align: center">PLATINUM</th>
                <th style="text-align: center">GOLD</th>
                <th style="text-align: center">SILVER</th>
                <th style="text-align: center">PRIZE/ BURSARY</th>
            </tr>
            <tr>
                <td>Standard Cost (from 1 September 2026)</td>
                <td align="center">£7500</td>
                <td align="center">£4500</td>
                <td align="center">£3000</td>
                <td align="center">£700</td>
                <td align="center">TBD</td>
            </tr>
            <tr>
                <td>Early Cost (to 31 August 2026)</td>
                <td align="center" vertical-align="middle">£3750</td>
                <td align="center">£2250</td>
                <td align="center">£1500</td>
                <td align="center">£650</td>
                <td align="center">TBD</td>
            </tr>
            <tr>
                <td style="vertical-align:middle">Logo and link on the conference website</td>
                <td align="center"><font style="color: rgb(181,18,27); font-size:125%">✔</font></td>
                <td align="center"><font style="color: rgb(181,18,27); font-size:125%">✔</font></td>
                <td align="center"><font style="color: rgb(181,18,27); font-size:125%">✔</font></td>
                <td align="center"><font style="color: rgb(181,18,27); font-size:125%">✔</font></td>
                <td align="center"><font style="color: rgb(181,18,27); font-size:125%">✔</font></td>
            </tr>
            <tr>
                <td style="vertical-align:middle">Logo on conference programme</td>
                <td align="center"><font style="color: rgb(181,18,27); font-size:125%">✔</font></td>
                <td align="center"><font style="color: rgb(181,18,27); font-size:125%">✔</font></td>
                <td align="center"><font style="color: rgb(181,18,27); font-size:125%">✔</font></td>
                <td align="center"><font style="color: rgb(181,18,27); font-size:125%">✔</font></td>
                <td align="center"><font style="color: rgb(181,18,27); font-size:125%">✔</font></td>
            </tr>
            <tr>
                <td style="vertical-align:middle">Covering 1 registration</td>
                <td align="center"><font style="color: rgb(181,18,27); font-size:125%">✔</font></td>
                <td align="center"><font style="color: rgb(181,18,27); font-size:125%">✔</font></td>
                <td align="center"><font style="color: rgb(181,18,27); font-size:125%">✔</font></td>
                <td align="center"><font style="color: rgb(181,18,27); font-size:125%">✔</font></td>
                <td align="center"><font style="color: rgb(192,192,192); font-size:125%">✘</font></td>
            </tr>
            <tr>
                <td style="vertical-align:middle">1 Exhibition stand</td>
                <td align="center"><font style="color: rgb(181,18,27); font-size:125%">✔</font></td>
                <td align="center"><font style="color: rgb(181,18,27); font-size:125%">✔</font></td>
                <td align="center"><font style="color: rgb(181,18,27); font-size:125%">✔</font></td>
                <td align="center"><font style="color: rgb(192,192,192); font-size:125%">✘</font></td>
                <td align="center"><font style="color: rgb(192,192,192); font-size:125%">✘</font></td>
            </tr>
            <tr>
                <td style="vertical-align:middle">Covering 1 additional free registration</td>
                <td align="center"><font style="color: rgb(181,18,27); font-size:125%">✔</font></td>
                <td align="center"><font style="color: rgb(181,18,27); font-size:125%">✔</font></td>
                <td align="center"><font style="color: rgb(192,192,192); font-size:125%">✘</font></td>
                <td align="center"><font style="color: rgb(192,192,192); font-size:125%">✘</font></td>
                <td align="center"><font style="color: rgb(192,192,192); font-size:125%">✘</font></td>
            </tr>
            <tr>
                <td style="vertical-align:middle">Acknowledgment in the opening address</td>
                <td align="center"><font style="color: rgb(181,18,27); font-size:125%">✔</font></td>
                <td align="center"><font style="color: rgb(181,18,27); font-size:125%">✔</font></td>
                <td align="center"><font style="color: rgb(192,192,192); font-size:125%">✘</font></td>
                <td align="center"><font style="color: rgb(192,192,192); font-size:125%">✘</font></td>
                <td align="center"><font style="color: rgb(181,18,27); font-size:125%">✔</font></td>
            </tr>
            <tr>
                <td style="vertical-align:middle">Promotion opportunity at the Welcome Reception</td>
                <td align="center"><font style="color: rgb(181,18,27); font-size:125%">✔</font></td>
                <td align="center"><font style="color: rgb(192,192,192); font-size:125%">✘</font></td>
                <td align="center"><font style="color: rgb(192,192,192); font-size:125%">✘</font></td>
                <td align="center"><font style="color: rgb(192,192,192); font-size:125%">✘</font></td>
                <td align="center"><font style="color: rgb(192,192,192); font-size:125%">✘</font></td>
            </tr>
            <tr>
                <td style="vertical-align:middle">Sponsorship of a Prize or Bursary</td>
                <td align="center"><font style="color: rgb(181,18,27); font-size:125%">✔</font></td>
                <td align="center"><font style="color: rgb(192,192,192); font-size:125%">✘</font></td>
                <td align="center"><font style="color: rgb(192,192,192); font-size:125%">✘</font></td>
                <td align="center"><font style="color: rgb(192,192,192); font-size:125%">✘</font></td>
                <td align="center"><font style="color: rgb(181,18,27); font-size:125%">✔</font></td>
            </tr>
        </tbody>
    </table>
</div>
