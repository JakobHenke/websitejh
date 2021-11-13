---
title: Gorilla Gorilla Gorilla 
subtitle: Teaching Students About Hypothesis Testing Should Include Visualizations

# Summary for listings and search engines
summary: Students should not only learn how to test hypothesis but how to visualize the data, too.

# Date published
date: "2021-11-13T00:00:00Z"

# Date updated
lastmod: "2021-11-13T00:00:00Z"

# Is this an unpublished draft?
draft: false

# Show this page in the Featured widget?
featured: false

# Featured image
# Place an image named `featured.jpg/png` in this page's folder and customize its options here.
image:
  caption: 'A hidden gorilla in a dataset, revealed by plotting media trust against conspiracy beliefs'
  focal_point: ""
  placement: 2
  preview_only: false

authors:
- admin

tags:
- Teaching

---

I am fascinated by gorillas. Some reasons are obvious. I mean…just look at them! I also absolutely adore the fact that the scientific name of the western lowland gorilla is simply *Gorilla Gorilla Gorilla*. How do you not come up with literally anything else when given the opportunity to name an animal?
Anyway, I recently came across [this editorial by Yanai & Lercher (2020)](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-020-02133-w) in which they argue that hypotheses can be liabilities because they prevent testers from discovering hidden patterns in data, thus potentially hindering scientific progress. They arrive at this inclusion based on an experiment in a statistics class:
They created a dataset with variables for participants’ Body Mass Index and steps they took in one day. They split this dataset into two, one for men and one for women in the sample. When plotted against each other in the whole dataset, the two variables revealed a picture of a waving gorilla, similar to the one above (in fact, both gorillas are based on the same image). The class was divided into two groups. One was told to explore the dataset, the other two test three hypotheses: 

1.	That the number of steps taken differs between men and women,
2.	that there is a negative correlation between the number of steps and BMI for women, and
3.	that there is a positive correlation between the two variables for men.

As it turns out, students in the first group were far more likely to find the gorilla. Now, there are many reasons to contest the authors’ conclusions. Some of which were published [in this response by Felin et al. (2021)](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-021-02276-4) (check out the response to the response [here](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-021-02277-3) if you’re interested).

I wouldn’t consider this a super rigorous experiment, but rather a fun, somewhat data-driven, anecdote about the point the authors are trying to make. And I agree that exploration is probably done too little, at least in communication and probably other social sciences as well. However, what caught my eye was the following quote from the first editorial:
“While we teach our students the benefits of visualization, answering the specific hypothesis-driven questions did not require plotting the data.”

As you may have guessed from the subtitle, I agree that visualizing data has many benefits. I disagree with the idea that it wasn’t necessary here. On the contrary, I think that visualizing the relationship between variables is a vital part of any hypothesis test, especially if the test has any built-in assumptions about what kind of relationship these variables have. Correlations coefficients, presumably what the students in the experiment calculated for H2 and H3, for example, aren’t particularly informative if the two variables don’t have a linear relationship. The easiest way to test this is by plotting the data. Take the two graphs below. One shows a clear quadratic, the other a cubic relationship. The Pearson correlations are -.07 and .88 respectively. In the case of the cubic, students who just calculate the correlation would falsely conclude that there is a strong (linear!) relationship between the two variables (here media trust and media cynicism). As for the quadratic, they would correctly conclude that there is no linear relationship between the variables (here media trust and media skepticism) but would miss the obvious non-linear relationship.

{{< figure src="cubic_quad.png">}}

Sure, observing such strong non-linear relationships in the utter wilderness that is social scientific data is rather unlikely. But my point is that we can only know this if we routinely visualize the relationships we hypothesize and test. This has nothing to do with exploration versus testing, but rather with due diligence while testing.

I try to teach my students exactly that. And that’s where the plots in this post come from. I generated a dataset with six variables and told them we had gathered these data in a recent survey. They had to first describe the individual variables (means, standard deviations, form of the univariate distributions) and then were told to test the correlations between the variables. Almost all students caught on to what was happening, especially after plotting political trust against political disenchantment.

{{< figure src="visualize.png">}}

Of course, this wasn’t a perfect or even conceptual replication of the original gorilla study. But I like to think that my conclusions would be the same if I had replicated the experiment as closely as possible.

Finally, I want to give a quick shout out to Magnus Karlsson whose [interactive visualization of correlations](https://rpsychologist.com/correlation/) always helps me to show what we can learn from a good graph.

And if you want to try something similar with your students, feel free to use or modify my dataset (link below). I told my students that all constructs were mean scores of five items measured from 1 to 10. Particularly observant students might realize that this makes some values impossible, but at least in my course, we didn’t dig in that deep. 

{{< icon name="download" pack="fas" >}} Download {{< staticref "uploads/data_gorilla.csv" "newtab" >}}the dataset{{< /staticref >}}.







