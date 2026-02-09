## Kiva Rwanda: Strategic Loan Analysis & Forecasting

Analyzed 3.7 years of Kiva crowdfunding data for Rwanda to identify operational trends and forecast annual performance.
Key Contributions:

- **Data Integrity & Logic:** Developed custom validation scripts to resolve inconsistencies in loan timestamps (posted vs. disbursed dates), ensuring data reliability.

- **Natural Language Processing (NLP):** Leveraged nltk to tokenize and analyze loan descriptions, identifying "buy targets" and sector-specific funding patterns.

- **Predictive Modeling:** Handled the 30% data gap in 2017 by using a timed index for my regression model, ensuring the forecast accounted for chronological trends rather than just raw averages, providing a more accurate estimation of year-over-year growth.

**Technical Stack:** Python (Pandas, Scikit-Learn, NLTK, Matplotlib/Seaborn), Git, and Linux-native development environments.

## Logic Patches & Iterations 05.02.26

The analysis evolved through several "logic-first" interventions where standard data cleaning wasn't enough:

- **The Currency 'Patch':** attempting to resolve 'currency consistency' using year-respective conversion rates led to collapse of predictive model. investigation revealed that the currency labels were simply metadata for the currency the loans were posted in and that all loans were disburesed in a single currency regardless.
        
- **The Borrowers’ Refinement:** revisited the entries under the borrower_genders column to make sense of list entries/multiple genders in one row. this led to consideration of welfare groups and saccos and groups in general as unique borrower categories. a clear relationship between group composition and size, and loan amount was established. 

- **Added a Table of Contents:** for easier navigation a clickable table of contents section is now present.
 