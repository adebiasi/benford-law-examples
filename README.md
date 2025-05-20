# Case Studies Using Benford's Law

Code adapted from the book [*Impractical Python Projects* by Lee Vaughan](https://www.penguinrandomhouse.com/books/568139/impractical-python-projects-by-lee-vaughan/).

## 2016 U.S. Presidential Election in Illinois

### Data Source

The official county-level results of the 2016 U.S. presidential election in Illinois are publicly available on [Wikipedia](https://en.wikipedia.org/wiki/2016_United_States_presidential_election_in_Illinois#By_county).

### Benford's Law Analysis

The following graphs show the distribution of the leading digits in the vote counts for each major candidate, compared against the expected distribution according to Benford's Law. Deviations from this expected pattern can suggest irregularities or simply reflect data characteristics (e.g., small sample sizes, constrained distributions).

---

#### Hillary Clinton

![Clinton First Digit Distribution](https://github.com/adebiasi/benford-law-examples/blob/main/generated_graphs/Percentage_First_Digits_Clinton.png)

**Interpretation**:  
Clinton’s vote distribution closely follows Benford’s Law. The first-digit frequencies largely align with the expected logarithmic curve, suggesting no apparent anomalies in the data.

---

#### Gary Johnson

![Johnson First Digit Distribution](https://github.com/adebiasi/benford-law-examples/blob/main/generated_graphs/Percentage_First_Digits_Johnson.png)

**Interpretation**:  
Johnson’s data shows significant deviation from Benford’s Law. However, this is likely due to the relatively low number of votes he received in most counties, resulting in a smaller and less varied dataset. Benford’s Law is less reliable for such limited ranges.

---

#### Jill Stein

![Stein First Digit Distribution](https://github.com/adebiasi/benford-law-examples/blob/main/generated_graphs/Percentage_First_Digits_Stein.png)

**Interpretation**:  
Like Johnson, Stein's vote totals are generally small across counties. The distribution of first digits deviates from Benford’s Law, but this is expected for datasets with low counts and limited numerical diversity.

---

#### Donald Trump

![Trump First Digit Distribution](https://github.com/adebiasi/benford-law-examples/blob/main/generated_graphs/Percentage_First_Digits_Trump.png)

**Interpretation**:  
Trump’s vote distribution shows noticeable deviations from Benford’s Law. Certain digits may appear more or less frequently than expected, suggesting that the data may not follow the natural logarithmic pattern. This could raise questions about irregularities or structural biases in the data. However, it's important to note that Benford’s Law is not a definitive test for fraud — deviations can also result from legitimate factors such as population distribution, voting patterns specific to certain counties, or reporting methods.

Further statistical analysis would be necessary to determine whether these deviations are significant or indicative of any anomalies beyond natural variance.


### Final Notes

Benford’s Law can be a useful tool for identifying data anomalies, but its results must be interpreted with caution. Not all deviations indicate fraud or errors—context, dataset size, and natural constraints all play a role in shaping digit distributions.
