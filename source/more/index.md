---
layout: page
menu_id: more
breadcrumb: false
comments: false
sidebar: subscriptions
---

{% navbar active:/more/ [我的订阅](/more/) [关于本站](/more/about/) [关于博主](/more/me/) %}
{% friends subscriptions %}

<hr/>
<br/>
<b>大佬们的最新博客</b>
{% grid %}
<!-- cell -->
{% timeline type:fcircle api:https://subscriptions.waddledee.com/all?rule=created&start=00&end=5 %}
{% endtimeline %}
<!-- cell -->
{% timeline type:fcircle api:https://subscriptions.waddledee.com/all?rule=created&start=5&end=10 %}
{% endtimeline %}
{% endgrid %}

<style>
  .md-text .tag-plugin.timeline .timenode>.body, .md-text .tag-plugin.timeline .timenode>.header {
    overflow: hidden;
    text-overflow: ellipsis;
    white-space: nowrap;
  }
</style>