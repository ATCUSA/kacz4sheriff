---
layout: page
title: Polling Places
permalink: /pollingplaces/
---

# Where to Vote
{: style="text-align: center;"}

### Boise County Polls will be open from 8 a.m. to 8 p.m.

If you know your precinct, you may look below for where to vote. If you are unsure, you can call the Boise County Clerk at 208-392-4431.

{% for place in site.data.pollingplaces %}
  <ul class="list-unstyled">
    <li>
      <h2><small>{{ place.precinct }}</small></h2>
      {{ place.location }}<br />
      {{ place.address }}<br />
      {{ place.town }}<br />
      {{ place.name }}
    </li>
  </ul>
{% endfor %}
