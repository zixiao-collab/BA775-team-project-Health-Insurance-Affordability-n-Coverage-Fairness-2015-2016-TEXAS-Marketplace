# BA775-team-project-Health-Insurance-Affordability-n-Coverage-Fairness-2015-2016-TEXAS-Marketplace
BA775 project analyzing Texas ACA Marketplace (2015–2016) with focus on insurance affordability, coverage fairness, and plan variation.

##  Project Overview

The analysis evaluates U.S. Marketplace Health Insurance data with a focused deep dive into Texas.  
Our goals include:

- **Premium affordability assessment**
- **Coverage fairness & benefit generosity comparison**
- **Insurer participation & competition stability**
- **Cost-sharing structure differences across states**

The project consists of:

- **Data preprocessing**
- **Feature engineering**
- **Tableau dashboard visualizations**
- **Clustering & statistical insights**

---

##  Data Source (BigQuery)

All datasets used in this project were prepared and joined in **Google BigQuery**.

###  Primary Table  
**`ba775b06teamproject.team.GEORGE_JOIN_TX`**

This unified table includes:

- **Rate PUF**: premiums by age & geography  
- **Benefits & Cost-Sharing PUF**: copays, coinsurance, MOOP, EHB coverage  
- **State-level economic indicators**  
- Derived metrics such as:  
  - **Relative Index** (affordability benchmark)  
  - **Premium Shock Ratio**  
  - **Competition Score**  

This table is the **single source of truth** for analysis, dashboards, and clustering.

---

##  Methodology

### **1. Data Cleaning & Integration**
- Removed missing / inconsistent records  
- Standardized column formats  
- Constructed derived variables  
- Joined all datasets in BigQuery  

### **2. Exploratory Data Analysis (EDA)**
- Distribution of premiums & cost-sharing  
- Age-rating curve comparison across states  
- Insurer entries/exits vs. premium volatility  
- Texas vs. national affordability benchmarking  

### **3. Dashboard Visualization**
Tableau dashboards highlight:

- **Age Banding by State**  
- **Median Standardized Premiums**  
- **Insurer Exit vs. Premium Shock**  
- **Out-of-Network Risk Map**  
- **Competition vs. Premium Volatility**  
- **Relative Index (vs. National Median)**  
- **Plan Clustering (Premium × Copay × Coinsurance)**  

### **4. Clustering Analysis**
Using premium, copay, and coinsurance:

- Identified **four plan clusters**  
- Revealed fairness & cost distribution patterns  
- Explored premium–benefit relationships  

---

##  Key Findings

- Texas has **mid-range premiums**, but **steep age-rating**, reducing affordability for older adults.  
- Higher premiums **do not guarantee** more generous benefits—cost-sharing varies significantly.  
- Despite many insurers, Texas maintains **stable premiums**, reflecting strong competition.  
- Out-of-network risks are **moderate**, still posing financial challenges for consumers.  

---
## Tableau Dashboard
### Dashboard 1
<div class='tableauPlaceholder' id='viz1765494495182' style='position: relative'><noscript><a href='#'><img alt='Dashboard 1 ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;BA&#47;BA775_Team_BigQuery_DashBoard_17652417831700&#47;Dashboard1&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='BA775_Team_BigQuery_DashBoard_17652417831700&#47;Dashboard1' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;BA&#47;BA775_Team_BigQuery_DashBoard_17652417831700&#47;Dashboard1&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='zh-CN' /></object></div>                <script type='text/javascript'>                    var divElement = document.getElementById('viz1765494495182');                    var vizElement = divElement.getElementsByTagName('object')[0];                    if ( divElement.offsetWidth > 800 ) { vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';} else if ( divElement.offsetWidth > 500 ) { vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';} else { vizElement.style.width='100%';vizElement.style.height='1877px';}                     var scriptElement = document.createElement('script');                    scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    vizElement.parentNode.insertBefore(scriptElement, vizElement);                </script>

### Dashboard 2
<div class='tableauPlaceholder' id='viz1765494548236' style='position: relative'><noscript><a href='#'><img alt='Dashboard 1 ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;81&#47;810teamproject1&#47;Dashboard1&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='810teamproject1&#47;Dashboard1' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;81&#47;810teamproject1&#47;Dashboard1&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='zh-CN' /></object></div>                <script type='text/javascript'>                    var divElement = document.getElementById('viz1765494548236');                    var vizElement = divElement.getElementsByTagName('object')[0];                    if ( divElement.offsetWidth > 800 ) { vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';} else if ( divElement.offsetWidth > 500 ) { vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';} else { vizElement.style.width='100%';vizElement.style.height='2177px';}                     var scriptElement = document.createElement('script');                    scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    vizElement.parentNode.insertBefore(scriptElement, vizElement);                </script>
---
##  Repository Structure

```
/notebooks/        Colab notebooks (EDA, SQL, clustering)
/sql/              BigQuery SQL scripts
/dashboards/       Tableau dashboard images & TWBX
/slides/           Final presentation (PDF)
/README.md         Project overview and documentation
```
---

##  Team

**BA775 – Team 06**

- Xincheng Ding  
- Tanmay Yenge  
- Zixiao Jiao  
- Linh Le  
- Yunhsuan Ku  
- Hanchao Tang  
