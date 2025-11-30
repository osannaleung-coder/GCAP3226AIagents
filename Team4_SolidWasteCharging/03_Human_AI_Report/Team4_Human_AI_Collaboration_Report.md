# Team 4: Human-AI Collaboration Report
## Food Waste Charging Scheme Analysis in Hong Kong


## Executive Summary (100-150 words)

Throughout GCAP3226, I used ChatGPT to analyze Hong Kong's citizens' food waste recycling habits and factors influencing their waste management behavior. My key insight is that effective human-AI collaboration requires combining ChatGPT's analytical capabilities with my essential domain knowledge about Hong Kong's waste challenges, primary survey data on recycling habits, and contextual understanding of local government policies. ChatGPT significantly accelerated my work on regression analysis and statistical modeling to identify relationships between recycling behavior and multiple factors including perceived government facilities, perceived barriers, food waste awareness, and demographics. I contributed irreplaceable elements: questionnaire design and data collection, interpretation of regression results for policy, and understanding of local government structures and recycling barriers. The most valuable aspect was using ChatGPT to implement sophisticated statistical analysis while maintaining human judgment over policy interpretation and recommendations.

---

## AI Usage Overview (200 words)

I strategically employed ChatGPT across different phases of my food waste recycling study. ChatGPT served as my primary analytical partner for brainstorming research questions, explaining regression statistics, suggesting statistical methodologies, and helping organize findings into clear structures.My usage patterns evolved significantly. In weeks 8-9, I used ChatGPT to help design my questionnaire and develop data collection strategies. In weeks 10-11 with questionnaire data ready, I increasingly relied on ChatGPT for technical analysis tasks—helping write Python code and explaining model specifications. In weeks 11-12, I used ChatGPT intensively to interpret regression results, understand relationships between recycling habits and perceived government facilities, identify which barriers most strongly predicted low recycling participation, and determine how food waste awareness influenced behavior across demographic groups. I used ChatGPT daily during data analysis and report writing phases.My specific ChatGPT use cases centered on four areas: First, code assistance for generating Python functions and calculating descriptive statistics. Second, methodology guidance on when to use logistic versus linear regression. Third, results interpretation—explaining what regression coefficients meant in policy terms. Fourth, report organization for non-technical audiences. Throughout this work, I validated ChatGPT-generated suggestions against my questionnaire data and course textbooks.

---

## Chat History Portfolio

### Key Chat Excerpts with Annotations

#### Chat 1: Methodology Selection (Week 10-11)

**My Question:**
"I have survey data on food waste recycling habits with a binary outcome variable (recycle yes/no) and multiple predictor variables including demographics, perceived government facilities, perceived barriers, and food waste awareness. Which regression model would be better—statistical (logistic) regression or linear regression? What are the advantages and disadvantages of each for my research question?"

**Why I Asked This:**
I needed to determine the most appropriate analytical method for my data structure. My outcome variable was categorical (binary), so I suspected logistic regression was appropriate, but I wanted ChatGPT to help me reason through the decision and understand the statistical implications.

**How I Used the Information:**
ChatGPT explained that logistic regression was better for binary outcomes because it models probabilities between 0 and 1, while linear regression assumes continuous outcomes and can produce impossible predictions outside this range. This directly informed my decision to use logistic regression for analyzing recycling participation.

**What I Modified or Validated:**
I validated this recommendation by reviewing my course textbook on regression methods and confirmed that logistic regression was indeed the correct choice for binary dependent variables. I then proceeded with logistic regression for all subsequent analyses.

**What I Learned:**
I learned the fundamental difference between outcome variable types and appropriate regression models. Understanding that model selection must match data characteristics deepened my statistical knowledge beyond simply applying formulas.

---

#### Chat 2: Code Development (Week 11)

**My Question:**
"Can you help me write Python code for a logistic regression model? I need to:
- Load my questionnaire data from a CSV file
- Prepare the data with my binary outcome variable (recycling: yes=1, no=0)
- Include predictor variables: age group, income level, perceived_facilities, perceived_barriers, food_waste_awareness
- Fit the logistic regression model
- Display coefficients and statistical significance
- Create a summary table showing odds ratios"

**Why I Asked This:**
I had identified the appropriate methodology but needed technical implementation. Rather than struggling with Python syntax alone, I asked ChatGPT to help generate the code structure, which I could then test and validate.

**How I Used the Information:**
ChatGPT provided a complete code template using scikit-learn and statsmodels libraries. I adapted this code by adding my specific variable names and data handling requirements. I tested the code against my actual questionnaire data and modified error handling based on issues encountered.

**What I Modified or Validated:**
I modified the original code to:
- Add data type checking for categorical variables
- Include dummy variable encoding for demographic groups
- Add model diagnostics checking (residual analysis, multicollinearity)
- Modify the odds ratio calculation to include 95% confidence intervals

I validated results by comparing coefficients with manual calculations for a subset of variables.

**What I Learned:**
I learned Python syntax for machine learning workflows, the importance of data preparation before modeling, and how to interpret logistic regression outputs including coefficients and odds ratios.

---

#### Chat 3: Visualization Development (Week 12)

**My Question:**
"Based on the results of my logistic regression model showing odds ratios and 95% confidence intervals for each predictor variable, can you help me write Python code to create a forest plot? I want to visualize:
- Each predictor variable on the y-axis
- Odds ratios with confidence intervals on the x-axis
- A vertical reference line at odds ratio = 1
- Clear labeling of variables and statistical significance"

**Why I Asked This:**
I had regression results but needed to communicate them visually to a non-technical audience. A forest plot is the standard visualization for regression results showing effect sizes and uncertainty. I asked ChatGPT to help implement this specific visualization.

**How I Used the Information:**
ChatGPT provided code using matplotlib and numpy to create a professional forest plot. I used this code to visualize my regression findings and identified which variables had odds ratios significantly different from 1 (confidence intervals not crossing 1.0).

**What I Modified or Validated:**
I modified the code to:
- Adjust color coding to highlight statistically significant predictors
- Add custom labels in policy terms (e.g., "Government Facility Access" instead of "perceived_facilities")
- Resize the plot for report inclusion
- Add a title and axis labels explaining the interpretation

I validated the plot by checking that odds ratios and confidence intervals matched my statistical output exactly.

**What I Learned:**
I learned how to communicate quantitative results visually and understood the importance of data visualization in policy communication. I recognized that effective forest plots require careful design choices about labeling and emphasis to support audience understanding.

---

### Prompting Skills Demonstrated

**Question 1** demonstrated context-rich prompting: I provided my specific data structure, outcome variable type, and analysis goals rather than asking a generic question.

**Question 2** showed iterative refinement: I followed up with specific requirements rather than requesting generic code.

**Question 3** exemplified task-specific prompting: I linked the visualization request directly to my analysis output and specified the audience (non-technical).

### Validation and Adaptation

Throughout these interactions, I maintained critical evaluation practices. When ChatGPT generated code, I:
- Tested it against actual data first
- Compared results against course materials
- Modified implementations based on specific data characteristics
- Validated statistical outputs through multiple approaches

This active engagement transformed ChatGPT from a shortcut tool into a genuine learning partner for statistical analysis and visualization.

---

## Reflection on Human-AI Collaboration (400 words)

I brought irreplaceable human contributions that ChatGPT could never provide. I designed and personally conducted questionnaires with residents across Hong Kong districts, gaining lived understanding of what "inconvenient pickup times" meant and recognizing patterns in how awareness varied by neighborhood and income level. I possessed Hong Kong-specific domain knowledge: understanding cultural attitudes toward food waste and recognizing practical implementation constraints. When ChatGPT helped me analyze regression coefficients showing that perceived government facilities strongly predicted recycling participation, I understood why from my questionnaire conversations—many residents didn't know facilities existed or found them difficult to access.

I deliberately used ChatGPT as a reasoning engine rather than an information source. Instead of asking generic questions, I prompted ChatGPT with specific scenarios: "Given these measured variables, what regression model would best test whether facility access matters more than cost barriers?" This approach made ChatGPT my analytical partner rather than a tool for generating answers.

I validated everything rigorously. I never trusted ChatGPT-suggested models without testing them against my actual questionnaire data first. I checked model assumptions by examining residual plots and testing for multicollinearity. When ChatGPT explained results, I compared those explanations against my course textbooks. I caught mistakes—for instance, when ChatGPT initially overlooked demographic interaction effects that I noticed in raw data.

My collaboration followed a clear pattern: ChatGPT generated analysis options, I applied critical judgment. Task division was natural—ChatGPT helped with coding and statistical explanation; I handled questionnaire design, data interpretation, and policy reasoning. When ChatGPT suggested certain variables weren't important, I overrode it with my domain knowledge about Hong Kong's urban density and infrastructure distribution.

My learning transformed through this collaboration. Before the course, I was skeptical that ChatGPT-assisted analysis would constitute real learning. I discovered that passive acceptance of ChatGPT outputs led to mistakes, but active engagement—reading explanations carefully, testing models, asking ChatGPT to explain reasoning—made it an effective learning partner. I learned regression analysis more deeply because I engaged with actual problems rather than abstract theory.

---

## Learning Outcomes and Transferable Skills (150 words)

This project developed significant skills for my professional career. I gained practical Python programming abilities for regression analysis, learned to specify regression models, and developed skills interpreting regression coefficients. I developed "AI literacy"—understanding how to write effective ChatGPT prompts, recognizing when outputs are reliable, and distinguishing between statistical and practical significance. I learned evidence-based environmental behavior analysis and how to connect regression findings to policy implications. Through questionnaire-based research, I practiced primary research methods and connecting quantitative results to qualitative understanding. My learning was accelerated by ChatGPT collaboration. I built multiple regression models quickly, compared specifications, and tested interaction effects. I learned regression diagnostics by solving actual problems with questionnaire data. These integrated skills—technical regression analysis, critical validation, primary research engagement, and human judgment—are essential for evidence-based careers where understanding both statistical relationships and human context matters.


