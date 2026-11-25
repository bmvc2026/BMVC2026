---
layout: default_sparse
title: Proceedings
permalink: /proceedings/
index: 5
---

{% assign sorted-papers = site.data.camera_ready.papers | sort: "number" %}

<div class="row pl-2 pr-2 pt-2 pb-2 mx-auto justify-content-left">
    <table class="table table-striped table-bordered" style="">
        <thead>
        <tr><th>ID</th><th>Paper</th></tr>
        </thead>
        <tbody>
            {% for paper in sorted-papers %}
            <!--{% assign all_authors = paper.authors | join: ", " %}-->
            {% assign all_authors = paper.authors | array_to_sentence_string %}
            <tr><td>{{paper.number}}</td>
            <td>
                <strong>{{paper.title}}</strong>
                <!--<br>{{all_authors}}-->
                <br>{% include authors.html authors=paper.authors %}
                <!--<br>
                {%- assign authors = paper.authors -%}
                {%- if authors.size > 1 -%}
                  {{ authors | pop | join: ", " }} and {{ authors | last }}
                {%- else -%}
                  {{ authors | first }}
                {%- endif -%}!-->
                <br>
                {%- assign padded_id = paper.number | prepend: "00000" | slice: -5, 5 -%}
                <!--<a class="btn btn-info btn-sm mt-1" href="{{ '/proceedings/papers/paper_' | append: padded_id | append: '/' | relative_url }}" role="button">Paper</a>&nbsp;-->
                <a class="btn btn-info btn-sm mt-1" href="https://www.bmva.org/bmvc/2026/proceedings/papers/paper_{{- padded_id -}}.html" role="button">Paper Page</a>&nbsp;
            </td></tr>
            {% endfor %}
        </tbody>
    </table>
</div>
