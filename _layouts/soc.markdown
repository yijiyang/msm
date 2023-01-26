---
layout: default
---
<h1>{{ page.name }}</h1>
<div class="soc">
<div class="content">
{{ content }}
</div>

<div class="soc-status">
<table>
<tr><td colspan="2">UART</td>{%include_cached status.liquid status=page.status-uart %}</tr>
<tr><td colspan="2">GCC</td>{%include_cached status.liquid status=page.status-gcc  %}</tr>
<tr><td colspan="2">Interconnect</td>{%include_cached status.liquid status=page.status-icc  %}</tr>
<tr><td colspan="2">GPU</td>{%include_cached status.liquid status=page.status-gpu  %}</tr>
<tr><td colspan="2">GPS</td>{%include_cached status.liquid status=page.status-gps  %}</tr>
<tr><td rowspan="4">Display</td>
  <td>MDP/DPU</td>{%include_cached status.liquid status=page.status-display-dpu  %}</tr>
  <tr><td>DSI</td>{%include_cached status.liquid status=page.status-display-dsi  %}</tr>
  <tr><td>HDMI</td>{%include_cached status.liquid status=page.status-display-hdmi  %}</tr>
  <tr><td>DP</td>{%include_cached status.liquid status=page.status-display-dp  %}</tr>
</table>
</div>

</div>
