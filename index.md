---
layout:     post
title:      Visual Analytics in Deep Learning
date:       2018-05-01 12:31:19
summary:    See what the different elements looks like. Your markdown has never looked better. I promise.
categories: jekyll pixyll
---

[Fred Hohman][fred], [Minsuk Khang][minsuk], [Robert Pienta][robert], [Duen Horng Chau][polo]

Deep learning has recently seen rapid development and significant attention due to its state-of-the-art performance on previously-thought hard problems. However, because of the innate complexity and nonlinear structure of deep neural networks, the underlying decision making processes for why these models are achieving such high performance are challenging and sometimes mystifying to interpret. As deep learning spreads across domains, it is of paramount importance that we equip users of deep learning with tools for understanding when a model works correctly, when it fails, and ultimately how to improve its performance. Standardized toolkits for building neural networks have helped democratize deep learning; visual analytics systems have now been developed to support model explanation, interpretation, debugging, and improvement.

<figure>
  <em>
  <img src="images/deepvis-6.png" style="border: 1px solid #eeeeee">
  </em>
</figure>

<!-- _![overview](images/deepvis-6.png)_ -->

We present a survey of the role of visual analytics in deep learning research, noting its short yet impactful history and summarize the state-of-the-art using a human-centered interrogative framework, focusing on the Five W’s and How (Why, Who, What, How, When, and Where), to thoroughly summarize deep learning visual analytics research. We conclude by highlighting research directions and open research problems. This survey helps new researchers and practitioners in both visual analytics and deep learning to quickly learn key aspects of this young and rapidly growing body of research, whose impact spans a diverse range of domains.

<table>

  <tr class="top-row">
    <td><div>&nbsp;</div></td>
    <td><div>&nbsp;</div></td>
    <td colspan="4" class="question-title"><div>Why</div></td>
    <!-- <td><div>asdf</div></td> -->
    <!-- <td><div>asdf</div></td> -->
    <!-- <td><div>asdf</div></td> -->
    <td colspan="3" class="question-title"><div>Who</div></td>
    <!-- <td><div>asdf</div></td> -->
    <!-- <td><div>asdf</div></td> -->
    <td colspan="5" class="question-title"><div>What</div></td>
    <!-- <td><div>asdf</div></td> -->
    <!-- <td><div>asdf</div></td> -->
    <!-- <td><div>asdf</div></td> -->
    <!-- <td><div>asdf</div></td> -->
    <td colspan="6" class="question-title"><div>How</div></td>
    <!-- <td><div>asdf</div></td> -->
    <!-- <td><div>asdf</div></td> -->
    <!-- <td><div>asdf</div></td> -->
    <!-- <td><div>asdf</div></td> -->
    <!-- <td><div>asdf</div></td> -->
    <td colspan="2" class="question-title"><div>When</div></td>
    <!-- <td><div>asdf</div></td> -->
    <td colspan="1" class="question-title"><div>Where</div></td>
  </tr>

  <tr>
    {% for field in site.data.fields %}  
      <td class="rotate"><div><span>{{ field.field }}</span></div></td>
    {% endfor %}
  </tr>

    {% for paper in site.data.papers %}
    <tr>

      <td>{{ paper.author }}</td>
      <td>{{ paper.year }}</td>

      {% if paper.interpretability            == 'x' %}<td class="checked"><span>&nbsp;</span></td>{% else %}<td></td>{% endif %}
      {% if paper.debugging                   == 'x' %}<td class="checked"><span>&nbsp;</span></td>{% else %}<td></td>{% endif %}
      {% if paper.comparing                   == 'x' %}<td class="checked"><span>&nbsp;</span></td>{% else %}<td></td>{% endif %}
      {% if paper.education                   == 'x' %}<td class="checked"><span>&nbsp;</span></td>{% else %}<td></td>{% endif %}
      {% if paper.model-developers            == 'x' %}<td class="checked"><span>&nbsp;</span></td>{% else %}<td></td>{% endif %}
      {% if paper.model-users                 == 'x' %}<td class="checked"><span>&nbsp;</span></td>{% else %}<td></td>{% endif %}
      {% if paper.non-experts                 == 'x' %}<td class="checked"><span>&nbsp;</span></td>{% else %}<td></td>{% endif %}
      {% if paper.graph                       == 'x' %}<td class="checked"><span>&nbsp;</span></td>{% else %}<td></td>{% endif %}
      {% if paper.learned                     == 'x' %}<td class="checked"><span>&nbsp;</span></td>{% else %}<td></td>{% endif %}
      {% if paper.units                       == 'x' %}<td class="checked"><span>&nbsp;</span></td>{% else %}<td></td>{% endif %}
      {% if paper.neurons                     == 'x' %}<td class="checked"><span>&nbsp;</span></td>{% else %}<td></td>{% endif %}
      {% if paper.aggregated                  == 'x' %}<td class="checked"><span>&nbsp;</span></td>{% else %}<td></td>{% endif %}
      {% if paper.node-link                   == 'x' %}<td class="checked"><span>&nbsp;</span></td>{% else %}<td></td>{% endif %}
      {% if paper.scatter                     == 'x' %}<td class="checked"><span>&nbsp;</span></td>{% else %}<td></td>{% endif %}
      {% if paper.line                        == 'x' %}<td class="checked"><span>&nbsp;</span></td>{% else %}<td></td>{% endif %}
      {% if paper.instance-based              == 'x' %}<td class="checked"><span>&nbsp;</span></td>{% else %}<td></td>{% endif %}
      {% if paper.interactive-experimentation == 'x' %}<td class="checked"><span>&nbsp;</span></td>{% else %}<td></td>{% endif %}
      {% if paper.algorithms                  == 'x' %}<td class="checked"><span>&nbsp;</span></td>{% else %}<td></td>{% endif %}
      {% if paper.during                      == 'x' %}<td class="checked"><span>&nbsp;</span></td>{% else %}<td></td>{% endif %}
      {% if paper.after                       == 'x' %}<td class="checked"><span>&nbsp;</span></td>{% else %}<td></td>{% endif %}

      <td> {{ paper.venue }} </td>
    </tr>
    {% endfor %}

</table>


## Citation

**Visual Analytics in Deep Learning: An Interrogative Survey for the Next Frontiers**  
Fred Hohman, Minsuk Kahng, Robert Pienta, Duen Horng Chau.  
*arXiv:1801.06889. Jan 21, 2018.*  

## BibTeX

{% highlight markdown %}
@article{hohman2017visual,
  title={Visual Analytics in Deep Learning: An Interrogative Survey for the Next Frontiers},
  author={Hohman, Fred and Kahng, Minsuk and Pienta, Robert and Chau, Duen Horng},
  journal={arXiv preprint arXiv:1801.06889},
  year={2018}
}
{% endhighlight %}

<!-- Markdown footnotes are supported, and they look great! Simply put e.g. `[^1]` where you want the footnote to appear,[^1] and then add -->
<!-- the reference at the end of your markdown. -->
<!-- <blockquote>
  <p>
    Perfection is achieved, not when there is nothing more to add, but when there is nothing left to take away.
  </p>
  <footer><cite title="Antoine de Saint-Exupéry">Antoine de Saint-Exupéry</cite></footer>
</blockquote> -->


---

[^1]: Important information that may distract from the main text can go in footnotes.

[fred]: www.fredhohman.com "Fred Hohnan."
[minsuk]: http://minsuk.com/ "Minsuk Kahng."
[robert]: http://spicy.bike/ "Robert Pienta."
[polo]: https://www.cc.gatech.edu/~dchau/ "Polo Chau."