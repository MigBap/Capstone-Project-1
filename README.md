# Capstone Project 1
Kiva loan delay analysis.

---
### Goal of the project:
Understand what may cause a higher delay between:
* the "posted time" (the time at which the loan is posted on Kiva by the field agent)
* the "funded time" (the time at which the loan posted to Kiva gets 100% funded by lenders)
* the "disbursed time" (the time at which the loan is disbursed by the field agent to the borrower)

<br>

**Method:** We see that there is a tendency to an increase on the fund delay over time, since the time it is posted or disbursed until the time it is funded or disbursed (see the files below for comprehension). To approach this problem, and after adjustments made regarding feature selection and engineering, I treated it as a classification problem, where the loan is either classified as with a "high delay" or "low delay".

### Files:

| File                                                         |    Description                                   |
| ------------------------------------------------------------ | ----------------------------------------------   |
| [Project proposal.pdf](https://github.com/MigBap/Springboard-Capstone-Project-I/blob/master/Capstone%20Project%201_%20Project%20Proposal.pdf)                                         |       Project proposal                           |
| [Capstone Project I -- 1) Data inspection and Cleaning.ipynb](http://bit.ly/2KdtLdF)  |       I part) Data inspection and Cleaning: code |
| [Capstone Project I -- 2) Exploratory Data Analysis.ipynb](http://bit.ly/2SLUa6c)     |       II part) Exploratory Data Analysis: code   |
| [Capstone Project I -- 3) Modeling.ipynb](http://bit.ly/2KaJI4A)                      |       III part) Modeling: code                   |
| [Capstone Project I -- All.ipynb](https://github.com/MigBap/Springboard-Capstone-Project-I/blob/master/Capstone%20Project%20I%20--%20All.ipynb)                              |       All code in one file                       |
| [Capstone Project I.pptx](https://github.com/MigBap/Springboard-Capstone-Project-I/blob/master/Capstone%20Project%20I.pptx)                                      |       PowerPoint presentation                    |
| [Capstone Project 1_Final report.pdf](https://github.com/MigBap/Springboard-Capstone-Project-I/blob/master/Capstone%20Project%201_Final%20report.pdf)                          |       Final report: Word document                |
| [data.txt](https://github.com/MigBap/Springboard-Capstone-Project-I/blob/master/data.txt)                                                     |       link for the data used                     |

<br>

**Conclusion:** The amount of the loan, the total number of lenders, the lender term and the currency policy are the most relevant features that explain loan delays. When relating to the EDA made, we see that some features are more helpful to predict when a loan will be delayed more than the desirable time, others to when it will have a smaller delay. For instance, the the two most important ones (loan amount and total number of lenders), which are positively correlated, help the explainability of the model in the sense that they contribute to higher delayed loans. Or, for instance, if it is a loan for Paraguay. Any loan with a high value in these features will be a motive of concern from the start, in the sense that they are good indicators of a higher delay. On the other hand, if, for instance, the loan has a shared currency policy, or it belongs to the 'Personal Use' sector, or the partner id is nº136, there is a good chance that the loan will be funded "on time". Considerations must also be taken regarding the correlation between these important variables, before concluding if a loan with this or that feature may be problematic, as explained in the documentation. 

