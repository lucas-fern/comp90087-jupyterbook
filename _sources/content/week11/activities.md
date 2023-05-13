# Tutorial 10 Activities

## Activities

```````{tab-set}
``````{tab-item} Task 1: Ofqual

Consider the following news article about *Ofqual*: an algorithmic approach that predict final grades for secondary school students in the England in 2020, who were unable to sit exams due to the COVID-19 pandemic.

```{epigraph}
[A-levels and GCSEs: How did the exam algorithm work?](https://www.bbc.com/news/explainers-53807730)

-- BBC News
```

*Ofqual* is/was a statistical model based on past performance that predicted final grades, which are used for university entrance, etc. At the time, after the predicted grades were released, there were protests from students and their families, leading to *Ofqual* not being used.


```{admonition} Exercise
:class: hint

In your group, discuss what information an explainability technique should give for *Ofqual*. Remember to think about relevant stakeholders in this scenario: who will want to know information about how *Ofqual* works. 
- Document at least three stakeholders and list what you think their primary goal should be for explainability of *Ofqual*. 
```
``````

``````{tab-item} Task 2: Credit Scoring
In financial institutions such as banks, *credit scoring models* have been used for decades to try to predict the risk of someone applying for a loan. These models use information such as: the loan amount requested, interest rate, term (length) of loan, age, previous loan information, current amount of debt, number of credit cards, occupation, education level, salary, and investments. 

Consider the three local explanations below for a business owner, Peta, who applied for a $12500 loan on a 24-month term at an interest rate of 12.5%. Peta has a credit rating of E (on a scale of A to F, where A is an excellent rating and F is a poor rating). Peta has run a successful business for five years and earns an annual salary of approximately $130,000.

Peta's primary goal in these explanations is recourse: to find out how to get a loan by either: (a) updating information that is incorrect; or (b) changing circumstances so that the next time, the loan is approved.


```{admonition} Exercise
:class: hint

In your group:
- Compare the three types of *local explanations* below and rank them for suitability based on whether they help Peta to achieve the goal of recourse. 
- Do you think the rankings would be the same for a data scientist building the credit scoring model? 
- Document your outcomes and justify your rankings. 
```
````

`````{tab-set}

````{tab-item} Attribution-based
Your loan application has been rejected in this instance. Here are the five most important reasons for this decision and their weights:

<table>
<thead>
  <tr>
    <th>Attribute</th>
    <th>Value</th>
    <th>Weight</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Salary</td>
    <td>$130,000</td>
    <td>2.9</td>
  </tr>
  <tr>
    <td>Interest rate</td>
    <td>12.5%</td>
    <td>-2.1</td>
  </tr>
  <tr>
    <td>Credit rating</td>
    <td>E</td>
    <td>2.0</td>
  </tr>
  <tr>
    <td>Loan term</td>
    <td>24 months</td>
    <td>1.9</td>
  </tr>
  <tr>
    <td>Occupation</td>
    <td>Business owner</td>
    <td>1.1</td>
  </tr>
</tbody>
</table>

Here, weight of the interest rate is negative because a higher interest rate makes the loan harder to pay off.
````

````{tab-item} Example-based (Prototypes)

Your loan application has been rejected in this instance. The following lists three examples of customers who have also had their loan rejected:

<table>
<thead>
  <tr>
    <th>Attribute</th>
    <th>Example customer 1</th>
    <th>Example customer 2</th>
    <th>Example customer 3</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Salary</td>
    <td>$120,000</td>
    <td>$80,000</td>
    <td>none</td>
  </tr>
  <tr>
    <td>Interest rate</td>
    <td>12.5%</td>
    <td>12.5%</td>
    <td>17.5%</td>
  </tr>
  <tr>
    <td>Credit rating</td>
    <td>E</td>
    <td>A</td>
    <td>D</td>
  </tr>
  <tr>
    <td>Loan term</td>
    <td>12 months</td>
    <td>60 months</td>
    <td>12 months</td>
  </tr>
  <tr>
    <td>Occupation</td>
    <td>Accountant</td>
    <td>Car restorer</td>
    <td>Author</td>
  </tr>
</tbody>
</table>
````

````{tab-item} Contrastive Explanation
Your loan application has been rejected in this instance. The following list four reasons why:

1. If your income had been $180,000 or above, you would have received the loan; *OR*
2. If you increased your loan term to 48 months, you would have received the loan; *OR*
3. If you applied for a small business loan, which has an interest rate of 9.5%, AND your income had been above $150,000, you would have received the loan; *OR*
4. If your occupation had been Chief Executive Officer, you would have received the loan.
````
`````
``````
```````

```{note}
As per usual, please remember to collate your answers and discussion points to these questions and post them in the [discussion board](https://canvas.lms.unimelb.edu.au/courses/151263/discussion_topics/870513)! :)
```
