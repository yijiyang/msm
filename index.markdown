---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---
<table>
<thead>
<tr>
<th rowspan="2">Platform</th>
<th rowspan="2">UART</th>
<th rowspan="2">GCC</th>
<th rowspan="2">Interconnect</th>
<th rowspan="2">GPU</th>
<th rowspan="2">GPS</th>
<th colspan="4">Display</th>
</tr>
<tr>
<th>MDP/DPU</th>
<th>DSI</th>
<th>HDMI</th>
<th>DP</th>
</tr>
</thead>
<tbody>
{% for d in site.soc %}
<tr>
<td><a href="{{d.url}}">{{d.name}}</a></td>
{%include_cached status.liquid status=d.status-uart %}
{%include_cached status.liquid status=d.status-gcc  %}
{%include_cached status.liquid status=d.status-icc  %}
{%include_cached status.liquid status=d.status-gpu  %}
{%include_cached status.liquid status=d.status-gps  %}
{%include_cached status.liquid status=d.status-display-dpu  %}
{%include_cached status.liquid status=d.status-display-dsi  %}
{%include_cached status.liquid status=d.status-display-hdmi  %}
{%include_cached status.liquid status=d.status-display-dp  %}
</tr>
{% endfor %}
</tbody>
</table>
