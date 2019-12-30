---
title: Publications
sectionid: publications
---

<h4>Selected publications (<a href="https://scholar.google.pl/citations?user=2oh_MFwAAAAJ&hl=en&oi=ao"><i>full list</i></a>)</h4>

We are committed to <a href="https://en.wikipedia.org/wiki/Open_access">open access</a>. If you find a manuscript that we have co-authored but is not available here, please <a href="/contactjoin">contact us</a> directly and we will be happy to send you an electronic copy.

<i>* Stands for first co-authorship</i><br>
<i># Stands for last co-authorship</i>
<hr>
<div class="container">
    {% for pub in site.papers reversed %} 
    <div class="row" > <div class="col-md-12">
    {{ pub }}
    </div></div>
    <hr>
    {% endfor %}
</div>