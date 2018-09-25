# Visual Analytics in Deep Learning
*An Interrogative Survey for the Next Frontiers*

This is the repository for the website of the TVCG 2018 survey paper on visual analytics in deep learning, presented at IEEE VIS 2018. 

**[Visual Analytics in Deep Learning: An Interrogative Survey for the Next Frontiers][site]**  
[Fred Hohman][fred], [Minsuk Kahng][minsuk], [Robert Pienta][robert], [Duen Horng Chau][polo].  
*IEEE Transactions on Visualization and Computer Graphics (TVCG). 2018.*  

## Add a new work

To add a new work to the table:

* Fork this repository.
* Edit the data file [`_data/works.yml`][works] by appending a new work to the very bottom of the file.
Use the following work as a template for adding the new work:
```yaml
- paper: kahng2018activis                  # lastname2018keyword
  url: http://minsuk.com/research/activis/ # project or paper link
  author: Kahng, et al.                    # abbreviated author list
  year: 2018                               # publication year

  # mark an `x` if a work belongs to a category and `o` if it doesn't
  why:
    - interpretability: x
      debugging: x
      comparing: o
      education: o
  who: 
    - model-developers: x
      model-users: x
      non-experts: o
  what:
    - graph: x
      learned: o
      units: x
      neurons: x
      aggregated: x
      node-link: x
  how: 
    - scatter: x
      line: o
      instance-based: x
      interactive-experimentation: o
      algorithms: o
  when:
    - during: o
      after: x
  where:
    - venue: TVCG                          # abbreviated publication venue
```
* Submit a [pull request][pull] with the newly added work.

## BibTeX

```latex
@article{hohman2018visual,
  title={Visual Analytics in Deep Learning: An Interrogative Survey for the Next Frontiers},
  author={Hohman, Fred and Kahng, Minsuk and Pienta, Robert and Chau, Duen Horng},
  journal={IEEE Transactions on Visualization and Computer Graphics},
  year={2018},
  publisher={IEEE}
}
```

## Credits

[Jekyll theme](http://www.pixyll.com) by [John Otander](http://johnotander.com).

[site]: https://fredhohman.com/visual-analytics-in-deep-learning
[fred]: https://fredhohman.com "Fred Hohman."
[minsuk]: http://minsuk.com/ "Minsuk Kahng."
[robert]: http://spicy.bike/ "Robert Pienta."
[polo]: https://www.cc.gatech.edu/~dchau/ "Polo Chau."

[works]: https://github.com/fredhohman/visual-analytics-in-deep-learning/blob/master/_data/works.yml "Works."
[pull]: https://github.com/fredhohman/visual-analytics-in-deep-learning/pulls "Make a new pull request."