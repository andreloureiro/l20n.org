---
category: learn
layout: learn
---

<section class="clearfix">
  <div class="left">
    <p>Let's say we want to translate the following string: <code>{% raw %}{{brandShortName}}{% endraw %} just crashed</code>.</p>
    <p>In Polish, the grammatical form of <code>crashed</code> depends on the gender of <code class="entity">brandShortName</code>. In order to construct a grammatically-correct and naturally-sounding message, we must know the gender of the subject.</p>
    <p>The localizer can define the gender (or, in fact, any arbitrary trait) as an attribute of the entity, so we can translate the example into Polish without sounding like a robot.</p>
  </div>
  <div class="right">
    <div class="editor sourceEditor height15"
      id="sourceEditor1"
      data-source="sourceEditor1"
      data-output="output1"
    >&lt;brandShortName "Boot2Gecko"
 _gender: "neutral"
&gt;
&lt;crashBanner[brandShortName::_gender] {
  masculine: "{% raw %}{{brandShortName}}{% endraw %} uległ awarii",
  feminine: "{% raw %}{{brandShortName}}{% endraw %} uległa awarii",
  neutral: "{% raw %}{{brandShortName}}{% endraw %} uległo awarii"
}&gt;
    </div>
    <dl id="output1">
    </dl>
  </div>
</section>
