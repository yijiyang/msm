---
layout: default
---
<h1>{{ page.name }}</h1>
<div class="pmic">
<div class="content">
{{ content }}
</div>

<div class="status">
<h2>Status</h2>
</div>

<table>
{% include layout_pmic.liquid %}
</table>

</div>
