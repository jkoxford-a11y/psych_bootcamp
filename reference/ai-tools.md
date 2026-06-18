---
layout: default
title: "AI Tools at a Glance"
permalink: /reference/ai-tools/
---

# AI Tools at a Glance

**Last updated: {{ site.data.ai-tools.last_updated }}**

Model names, pricing, and features change frequently. If something here looks wrong, it probably is — check the provider's website.

*To update this table: edit `_data/ai-tools.yml`. The page regenerates automatically.*

---

<table>
<thead>
<tr>
<th>Tool</th>
<th>Provider</th>
<th>Free tier</th>
<th>Paid tier</th>
<th>Strengths for faculty</th>
</tr>
</thead>
<tbody>
{% for tool in site.data.ai-tools.tools %}
<tr>
<td><strong>{{ tool.name }}</strong></td>
<td>{{ tool.provider }}</td>
<td>{{ tool.free_tier }}</td>
<td>{{ tool.paid_tier }}</td>
<td>{{ tool.strengths }}</td>
</tr>
{% endfor %}
</tbody>
</table>

---

[← Back to home]({{ site.baseurl }}/)
