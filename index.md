---
layout:     post
title:      Visual Analytics in Deep Learning
date:       2018-05-01 12:31:19
summary:    See what the different elements looks like. Your markdown has never looked better. I promise.
categories: jekyll pixyll
---

[Fred Hohman][fred], [Minsuk Kahng][minsuk], [Robert Pienta][robert], [Duen Horng Chau][polo]

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

    <td colspan="4" class="question-title" id="why-title"><div>WHY</div></td>
    <!-- <td><div>asdf</div></td> -->
    <!-- <td><div>asdf</div></td> -->
    <!-- <td><div>asdf</div></td> -->

    <td colspan="3" class="question-title" id="who-title"><div>WHO</div></td>
    <!-- <td><div>asdf</div></td> -->
    <!-- <td><div>asdf</div></td> -->

    <td colspan="5" class="question-title" id="what-title"><div>WHAT</div></td>
    <!-- <td><div>asdf</div></td> -->
    <!-- <td><div>asdf</div></td> -->
    <!-- <td><div>asdf</div></td> -->
    <!-- <td><div>asdf</div></td> -->

    <td colspan="6" class="question-title" id="how-title"><div>HOW</div></td>
    <!-- <td><div>asdf</div></td> -->
    <!-- <td><div>asdf</div></td> -->
    <!-- <td><div>asdf</div></td> -->
    <!-- <td><div>asdf</div></td> -->
    <!-- <td><div>asdf</div></td> -->

    <td colspan="2" class="question-title" id="when-title"><div>WHEN</div></td>
    <!-- <td><div>asdf</div></td> -->

    <td colspan="1" class="question-title" id="where-title"><div>WHERE</div></td>

  </tr>

<!-- <tr class="bordered">&nbsp;</tr> -->

  <tr>
    {% for field in site.data.fields %}  
      <td class="rotate"><div><span>{{ field.field }}</span></div></td>
    {% endfor %}
  </tr>

    {% for work in site.data.works %}
    <tr>

      <td class="author">{{ work.author }}</td>
      <td class="year">{{ work.year }}</td>

      {% if work.interpretability            == 'x' %}<td class="checked interpretability"><span>&nbsp;</span></td>{% else %}<td class="interpretability"></td>{% endif %}
      {% if work.debugging                   == 'x' %}<td class="checked debugging"><span>&nbsp;</span></td>{% else %}<td class="debugging"></td>{% endif %}
      {% if work.comparing                   == 'x' %}<td class="checked comparing"><span>&nbsp;</span></td>{% else %}<td class="comparing"></td>{% endif %}
      {% if work.education                   == 'x' %}<td class="checked education"><span>&nbsp;</span></td>{% else %}<td class="education"></td>{% endif %}
      {% if work.model-developers            == 'x' %}<td class="checked model-developers"><span>&nbsp;</span></td>{% else %}<td class="model-developers"></td>{% endif %}
      {% if work.model-users                 == 'x' %}<td class="checked model-users"><span>&nbsp;</span></td>{% else %}<td class="model-users"></td>{% endif %}
      {% if work.non-experts                 == 'x' %}<td class="checked non-experts"><span>&nbsp;</span></td>{% else %}<td class="non-experts"></td>{% endif %}
      {% if work.graph                       == 'x' %}<td class="checked graph"><span>&nbsp;</span></td>{% else %}<td class="graph"></td>{% endif %}
      {% if work.learned                     == 'x' %}<td class="checked learned"><span>&nbsp;</span></td>{% else %}<td class="learned"></td>{% endif %}
      {% if work.units                       == 'x' %}<td class="checked units"><span>&nbsp;</span></td>{% else %}<td class="units"></td>{% endif %}
      {% if work.neurons                     == 'x' %}<td class="checked neurons"><span>&nbsp;</span></td>{% else %}<td class="neurons"></td>{% endif %}
      {% if work.aggregated                  == 'x' %}<td class="checked aggregated"><span>&nbsp;</span></td>{% else %}<td class="aggregated"></td>{% endif %}
      {% if work.node-link                   == 'x' %}<td class="checked node-link"><span>&nbsp;</span></td>{% else %}<td class="node-link"></td>{% endif %}
      {% if work.scatter                     == 'x' %}<td class="checked scatter"><span>&nbsp;</span></td>{% else %}<td class="scatter"></td>{% endif %}
      {% if work.line                        == 'x' %}<td class="checked line"><span>&nbsp;</span></td>{% else %}<td class="line"></td>{% endif %}
      {% if work.instance-based              == 'x' %}<td class="checked instance-based"><span>&nbsp;</span></td>{% else %}<td class="instance-based"></td>{% endif %}
      {% if work.interactive-experimentation == 'x' %}<td class="checked interactive-experimentation"><span>&nbsp;</span></td>{% else %}<td class="interactive-experimentation"></td>{% endif %}
      {% if work.algorithms                  == 'x' %}<td class="checked algorithms"><span>&nbsp;</span></td>{% else %}<td class="algorithms"></td>{% endif %}
      {% if work.during                      == 'x' %}<td class="checked during"><span>&nbsp;</span></td>{% else %}<td class="during"></td>{% endif %}
      {% if work.after                       == 'x' %}<td class="checked after"><span>&nbsp;</span></td>{% else %}<td class="after"></td>{% endif %}

      <td class="venue"> {{ work.venue }} </td>

    </tr>
    {% endfor %}

</table>


## Citation

**Visual Analytics in Deep Learning: An Interrogative Survey for the Next Frontiers**  
Fred Hohman, Minsuk Kahng, Robert Pienta, Duen Horng Chau.  
*arXiv:1801.06889. Jan 21, 2018.*  

## BibTeX

```latex
@article{hohman2017visual,
  title={Visual Analytics in Deep Learning: An Interrogative Survey for the Next Frontiers},
  author={Hohman, Fred and Kahng, Minsuk and Pienta, Robert and Chau, Duen Horng},
  journal={arXiv preprint arXiv:1801.06889},
  year={2018}
}
```

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