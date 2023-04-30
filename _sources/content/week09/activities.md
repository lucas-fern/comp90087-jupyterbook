# Tutorial 9 Activities

## Activities

`````{tab-set}
````{tab-item} Task 1: Correlation and Bias?

Assuming you have a large tech company, say, Apple, who has a prestigious tech internship program for Year 12 graduates.

In the first round of applications, we have six candidates, but only two are successful.

**This is mainly determined by an average score (*HR Panel Average Score* - from 0.0 to 10.0) across a panel of judges and expert HR recruiters at Apple -- to clarify, this overall score is determined by humans (e.g., the average of scores given by the individual judges and recruiters).**

This table contains some data about the candidates, including the proposed undergraduate degree major they have shortlisted for their uni degree, and achievements to date.

<table>
<thead>
  <tr>
    <th>Outcome</th>
    <th>HR Panel Average Score</th>
    <th>First Name</th>
    <th>Surname</th>
    <th>School</th>
    <th>Proposed University Major</th>
    <th>Achievements</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Hired</td>
    <td>9.56</td>
    <td>Jack</td>
    <td>Brigs</td>
    <td>Caulfield Boys School</td>
    <td>Software Engineering</td>
    <td>Cycling Champion</td>
  </tr>
  <tr>
    <td>Hired</td>
    <td>9.22</td>
    <td>Jackson</td>
    <td>Singh</td>
    <td>Geelong Boys College</td>
    <td>Science</td>
    <td>Marathon Runner Up</td>
  </tr>
  <tr>
    <td>Not Hired</td>
    <td>8.62</td>
    <td>Marie</td>
    <td>Currie</td>
    <td>Newtown Public School</td>
    <td>Mathematics</td>
    <td>Junior MasterChef Winner</td>
  </tr>
  <tr>
    <td>Not Hired</td>
    <td>8.50</td>
    <td>Gabi</td>
    <td>Miller</td>
    <td>Sydney North College</td>
    <td>Philosophy</td>
    <td>Rotary Club Award Recipient</td>
  </tr>
  <tr>
    <td>Not Hired</td>
    <td>7.83</td>
    <td>Sandra</td>
    <td>Lee</td>
    <td>Bondi Girls College</td>
    <td>Mass Communications</td>
    <td>X Factor Runner Up / Australian Idol Finalist</td>
  </tr>
  <tr>
    <td>Not Hired</td>
    <td>4.55</td>
    <td>Trinity</td>
    <td>Reeves</td>
    <td>Parramatta Girls High School</td>
    <td>Fine Art</td>
    <td>Heidelberg Art Show Winner</td>
  </tr>
</tbody>
</table>

To us humans, we know that the **HR Panel Average Score** is the only thing that determined their outcome, as mentioned before in bold. Everything else is just coincidental, especially on a data set this small.

There are potential problems if the data set (of human judgement) is used for creating ML models to replace the human HR panel in predicting future outcomes. (Hint: read the Amazon Case Study in the Readings/Videos this week - Amazon did a similar thing!).

However, [spurious correlations](https://en.wikipedia.org/wiki/Spurious_relationship) do exist in this dataset. If a naive classifier (e.g. using frequency of words, word embedding techniques) is trained on this dataset, a spurious connection can be as follows:

*"Those whose first names contain 'Jack' will be hired 100% of the time"*

Of course - this is false!

```{admonition} Exercise
:class: hint
In your group, based on this observation, as well as hypothetical uses of this dataset for building ML models (as above), discuss the following:

1. What is the meaning of the maxim *correlation does not imply causation*? Hence, *what are spurious relationships/spurious correlations*? Explain with an example taken from, e.g. [here](https://tylervigen.com/page?page=2Links) or [here](https://en.wikipedia.org/wiki/Correlation_does_not_imply_causation) (or any other example you can think about).

2. Over time, if this classifier model is to be used for shortlisting actual job candidates at Apple, indicate what other spurious correlations it can find. More importantly:
    - how do these entrench biases (both machine bias, and societal bias) that disadvantage people in particular groups or of particular characteristics? 
        - Consider *discriminatory bias* (with job fit, gender) and also spurious correlations (e.g. does it look like certain schools in certain regions are advantaged?) 
    - are there any features which are acceptable for use?
```
````

````{tab-item} Task 2: Contactless Parking Apps

```{note}
As discussed in this week's Modules, accessibility is more than assisting people living with disabilities; consider also issues such as situational impairments. Sometimes, issues with accessibility are interrelated with issues concerning equity of AI systems
```

After the pandemic, 'contactless' technologies have been promoted in Australia and other countries, to reduce the need of handling cash, as well as avoid human contact with surfaces such as credit card readers. Thereby, this promotes physical distancing and avoiding the touching of surfaces, to help reduce the spread of Covid-19.

Many public parking systems in various suburbs are thus equipped with a 'contactless' way to pay for parking, say by using a smartphone app, or a web browser-based app. These often require the storage of credit card details with the app provider. Assume some of these systems completely replace traditional systems, including credit card terminals, pay-to-park (coins and bank notes) terminals, or a human-staffed parking booth.

```{admonition} Exercise
:class: hint
In your group, discuss the case above with reference to accessibility and equity. To get started, here are some potential stakeholders which may be negatively impacted:
- Equity: people without smartphones or technical expertise;
- Equity: people who cannot obtain credit cards;
- Accessibility: people who can't use their phone screen due to risk of migraines;
- Accessibility: busy parents who are juggling both family/carer responsibilities with work.
```
````
`````

```{note}
We look forward to seeing your amazing contributions on the [forum discussion](https://canvas.lms.unimelb.edu.au/courses/151263/discussion_topics/870509).
```
