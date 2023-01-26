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
<tr><td>GPIO</td>{%include_cached status.liquid status=page.pmic-gpio %}</tr>
<tr><td>MPP</td>{%include_cached status.liquid status=page.pmic-mpp %}</tr>
<tr><td>RTC</td>{%include_cached status.liquid status=page.pmic-rtc %}</tr>
<tr><td>ADC</td>{%include_cached status.liquid status=page.pmic-adc %}</tr>
<tr><td>ADC-TM</td>{%include_cached status.liquid status=page.pmic-adc-tm %}</tr>
<tr><td>temp-alarm</td>{%include_cached status.liquid status=page.pmic-temp-alarm %}</tr>
</table>

</div>
