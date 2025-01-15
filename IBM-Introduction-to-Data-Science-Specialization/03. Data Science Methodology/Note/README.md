# 3. Data Science Methodology

---

# Week01 - From Problem to Approach and From Requirements to Collectio

### Pre

![Untitled](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/Untitled.png)

![Untitled](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/Untitled%201.png)

- CRISP-DM methodology
    - Cross Industry Process for Data Mining (CRISP-DM) methodology
        - 跨行业数据挖掘标准流程
    - used by data mining, business application
    - 6 steps
        
        ![DS_3.1.0.5-CRISP-DM-Model-2.png](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/DS_3.1.0.5-CRISP-DM-Model-2.png)
        
        1. **Business Understanding** This stage is the most important because this is where the intention of the project is outlined. Foundational Methodology and CRISP-DM are aligned here. It requires communication and clarity. The difficulty here is that stakeholders have different objectives, biases, and modalities of relating information. They don’t all see the same things or in the same manner. Without clear, concise, and complete perspective of what the project goals are resources will be needlessly expended.
        2. **Data Understanding** Data understanding relies on business understanding. Data is collected at this stage of the process. The understanding of what the business wants and needs will determine what data is collected, from what sources, and by what methods. CRISP-DM combines the stages of Data Requirements, Data Collection, and Data Understanding from the Foundational Methodology outline.
        3. **Data Preparation** Once the data has been collected, it must be transformed into a useable subset unless it is determined that more data is needed. Once a dataset is chosen, it must then be checked for questionable, missing, or ambiguous cases. Data Preparation is common to CRISP-DM and Foundational Methodology.
        4. **Modeling** Once prepared for use, the data must be expressed through whatever appropriate models, give meaningful insights, and hopefully new knowledge. This is the purpose of data mining: to create knowledge information that has meaning and utility. The use of models reveals patterns and structures within the data that provide insight into the features of interest. Models are selected on a portion of the data and adjustments are made if necessary. Model selection is an art and science. Both Foundational Methodology and CRISP-DM are required for the subsequent stage.
        5. **Evaluation** The selected model must be tested. This is usually done by having a pre-selected test, set to run the trained model on. This will allow you to see the effectiveness of the model on a set it sees as new. Results from this are used to determine efficacy of the model and foreshadows its role in the next and final stage.
        6. **Deployment** In the deployment step, the **model is used on new data outside of the scope of the dataset** and by **new stakeholders**. The new interactions at this phase might reveal the new variables and needs for the dataset and model. These new challenges could initiate revision of either business needs and actions, or the model and data, or both.
        - Pros:
            - flexiable

### From Problem to Approach

- **Business Understanding**
    - Rollins suggests that having a clearly defined question is vital because it ultimately directs the analytic approach that will be needed to address the question.
    - Case Study
        - Problems:
            - What is the best way to allocate the limited healthcare budget to maximize its use in providing quality care?
        - **Vital!** - What are the goals and objectives
            - Define the goals
                - To provide quality care without incearsing costs
            - Define the objectives
                - To review the process to identify inefficiencies
        - Conclusion
        - What is the sponsor’s involvement?
            - set overall direction
            - remained engaged and provide guidance
            - ensured necessary support, where needed
        - identifying the business requirements
            
            ![Untitled](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/Untitled%202.png)
            
            - Predicting readmission outcomes for those patients with Congestive Heart Failure Predicting readmission risk.
            - Understanding the combination of events that led to the predicted outcome
            - Applying an easy-to-understand process to new patients, regarding their readmission risk.
            - 
- **Analytic Approach**
    - Once the problem to be addressed is defined, the appropriate analytic approach for the problem is selected in the context of the business requirements.
    
    ![Untitled](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/Untitled%203.png)
    
    ![Untitled](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/Untitled%204.png)
    
    - Case Study
        
        ![Untitled](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/Untitled%205.png)
        
        ![Untitled](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/Untitled%206.png)
        
- Lab
    - [ ]  Done?
    
    [DS0103EN-Exercise-From-Problem-to-Approach.ipynb](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/DS0103EN-Exercise-From-Problem-to-Approach.ipynb)
    
- Summary
    - The need to understand and prioritize the business goal.
    - The way stakeholder support influences a project.
    - The importance of selecting the right model.
    - When to use a predictive, descriptive, or classification model.

### From Requirements to Collectio

![Untitled](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/Untitled%207.png)

- **Data Requirements**
    - **Case Study**
        
        ![Untitled](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/Untitled%208.png)
        
        ![Untitled](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/Untitled%209.png)
        
- **Data Collection**
    - a follow-up to the data requirements stage
    - Case Study
        
        ![Untitled](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/Untitled%2010.png)
        
        ![Untitled](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/Untitled%2011.png)
        
        ![Untitled](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/Untitled%2012.png)
        
- Lab
    - [ ]  Done?
    
    [DS0103EN-Review-From-Requirements-to-Collection.ipynb](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/DS0103EN-Review-From-Requirements-to-Collection.ipynb)
    
- Summary
    - The significance of defining the data requirements for your model.
    - Why the content, format, and representation of your data matter.
    - The importance of identifying the correct sources of data for your project.
    - How to handle unavailable and redundant data.
    - To anticipate the needs of future stages in the process.

# Week02 - From Understanding to Preparation and From Modeling to Evaluation

- Data Understanding
- Data Preparation
- Modeling
- Evaluation

### Pre

### **Learning Objectives**

---

- Prepare a data set by handling missing, invalid, or misleading data.
- Describe the purpose and characteristics of the data modeling process.
- Evaluate a decision tree model using a training and a test dataset.
- Build a decision to tree to determine the cuisine type for a data set of recipes.
- Summarize the processes of understanding data preparing data, modeling, and evaluation phases of the data science methodology.

### **From Understanding to Preparation**

- **Data Understanding**
    
    ![Untitled](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/Untitled%2013.png)
    
    - Question: Is the data that you collected representative of the problem to be solved?
    - **[Descriptive Statistics](https://www.investopedia.com/terms/d/descriptive_statistics.asp)**
    
    ![Untitled](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/Untitled%2014.png)
    
    - Histograms(**直方圖**) are a good way to understand how values or a variable are distributed, and which sorts of data preparation may be needed to make the variable more useful in a model.
    
    ![Untitled](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/Untitled%2015.png)
    
    - The univariates, statistics, and histograms are also used to assess data quality.
    - A certain valuable has missing anything?
        - Question → Does missing mean anything?
            - Sometimes a missing value might be “no”, “0”, “NULL”
            - or invalid or misleading value e.g. age = 999 → no meaning
    
    ![Untitled](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/Untitled%2016.png)
    
- **Data Preparation**
    - Concept
        - **cleansing data**
        - Data preparation is the most time consuming phase of a data scinece project (70% - 90 % project time)
        
        ![Untitled](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/Untitled%2017.png)
        
        - Data preparation stage answers: What are the ways in which data is prepared?
        
        ![Untitled](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/Untitled%2018.png)
        
        ![Untitled](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/Untitled%2019.png)
        
    - Case Study
        
        ![Untitled](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/Untitled%2020.png)
        
        ![Untitled](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/Untitled%2021.png)
        
        ![Untitled](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/Untitled%2022.png)
        
        ![Untitled](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/Untitled%2023.png)
        
        ![Untitled](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/Untitled%2024.png)
        
        ![Untitled](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/Untitled%2025.png)
        
        ![Untitled](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/Untitled%2026.png)
        
        ![Untitled](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/Untitled%2027.png)
        
        ![Untitled](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/Untitled%2028.png)
        
        - Explanation (EN)
            
            In a sense, data preparation is similar to washing freshly picked vegetables insofar as unwanted elements, such as dirt or imperfections, are removed. So now, let's look at the case study related to applying Data Preparation concepts. In the case study, an important first step in the data preparation stage was to actually define congestive heart failure. This sounded easy at first but defining it precisely, was not straightforward. First, the set of diagnosis-related group codes needed to be identified, as congestive heart failure implies certain kinds of fluid buildup. We also needed to consider that congestive heart failure is only one type of heart failure. Clinical guidance was needed to get the right codes for congestive heart failure. The next step involved defining the re-admission criteria for the same condition. The timing of events needed to be evaluated in order to define whether a particular congestive heart failure admission was an initial event, which is called an index admission, or a congestive heart failure-related re-admission. Based on clinical expertise, a time period of 30 days was set as the window for readmission relevant for congestive heart failure patients, following the discharge from the initial admission. Next, the records that were in transactional format were aggregated, meaning that the data included multiple records for each patient. Transactional records included professional provider facility claims submitted for physician, laboratory, hospital, and clinical services. Also included were records describing all the diagnoses, procedures, prescriptions, and other information about in-patients and out-patients. A given patient could easily have hundreds or even thousands of these records, depending on their clinical history. Then, all the transactional records were aggregated to the patient level, yielding a single record for each patient, as required for the decision-tree classification method that would be used for modeling. As part of the aggregation process, many new columns were created representing the information in the transactions. For example, frequency and most recent visits to doctors, clinics and hospitals with diagnoses, procedures, prescriptions, and so forth. Co-morbidities with congestive heart failure were also considered, such as diabetes, hypertension, and many other diseases and chronic conditions that could impact the risk of re-admission for congestive heart failure. During discussions around data preparation, a literary review on congestive heart failure was also undertaken to see whether any important data elements were overlooked, such as co-morbidities that had not yet been accounted for. The literary review involved looping back to the data collection stage to add a few more indicators for conditions and procedures. Aggregating the transactional data at the patient level, meant merging it with the other patient data, including their demographic information, such as age, gender, type of insurance, and so forth. The result was the creation of one table containing a single record per patient, with many columns representing the attributes about the patient in his or her clinical history. These columns would be used as variables in the predictive modeling. Here is a list of the variables that were ultimately used in building the model. The dependent variable, or target, was congestive heart failure readmission within 30 days following discharge from a hospitalization for congestive heart failure, with an outcome of either yes or no. The data preparation stage resulted in a cohort of 2,343 patients meeting all of the criteria for this case study. The cohort was then split into training and testing sets for building and validating the model, respectively. This ends the Data Preparation section of this course, in which we applied the key concepts to the case study.
            
        - Explanation (ZH)
            
            從某種意義上說，數據準備類似於清洗新採摘的蔬菜，因為不需要的元素，如灰塵或瑕疵，都會被去除。那麼現在，讓我們來看看與應用數據準備概念有關的案例研究。在該案例研究中，數據準備階段的重要第一步是實際定義充血性心力衰竭。這起初聽起來很容易，但準確定義它，並不簡單。首先，需要確定與診斷相關的一組代碼，因為充血性心力衰竭意味著某些類型的液體堆積。我們還需要考慮，充血性心力衰竭只是心力衰竭的一種類型。為了獲得正確的充血性心力衰竭的編碼，需要有臨床指導。下一步是定義同一條件下的再入院標準。需要對事件發生的時間進行評估，以確定某一充血性心力衰竭入院是初始事件，即所謂的指數入院，還是充血性心力衰竭相關的再次入院。根據臨床專業知識，在初次入院出院後，30天的時間段被設定為與充血性心力衰竭患者有關的再入院窗口。接下來，交易格式的記錄被匯總，也就是說，數據包括每個病人的多個記錄。交易記錄包括專業供應商設施提交的醫生、實驗室、醫院和臨床服務的索賠。還包括描述所有診斷、程序、處方和其他住院病人和門診病人信息的記錄。根據他們的臨床病史，一個特定的病人可能很容易有數百甚至數千條這樣的記錄。然後，所有的交易記錄被匯總到病人層面，產生每個病人的單一記錄，這是用於建模的決策樹分類方法的要求。作為匯總過程的一部分，許多新的列被創建，代表交易中的信息。例如，醫生、診所和醫院的就診頻率和最近的就診情況，包括診斷、程序、處方等等。還考慮了與充血性心力衰竭有關的共病，如糖尿病、高血壓，以及其他許多可能影響充血性心力衰竭再入院風險的疾病和慢性病。在圍繞數據準備的討論中，還進行了關於充血性心力衰竭的文學評論，以了解是否有任何重要的數據元素被忽略，如尚未被考慮的合併疾病。文獻審查涉及回溯到數據收集階段，以增加一些條件和程序的指標。在病人層面匯總交易數據，意味著將其與其他病人數據合併，包括他們的人口信息，如年齡、性別、保險類型等。其結果是創建一個表，包含每個病人的一條記錄，其中有許多列代表病人在其臨床歷史中的屬性。這些列將被用作預測模型的變量。以下是最終用於建立模型的變量列表。因變量或目標是充血性心力衰竭出院後30天內的再入院情況，其結果是有或無。數據準備階段產生了一個符合本案例研究所有標準的2,343名患者隊列。然後，該隊列被分成訓練集和測試集，分別用於建立和驗證該模型。本課程的數據準備部分到此結束，在這部分中我們將關鍵概念應用於案例研究。
            
- Lab
    - [ ]  Done?
    
    [DS0103EN-Exercise-From-Understanding-to-Preparation.ipynb](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/DS0103EN-Exercise-From-Understanding-to-Preparation.ipynb)
    
- Lesson Summary
    
    In this lesson, you have learned:
    
    - The importance of descriptive statistics.
    - How to manage missing, invalid, or misleading data.
    - The need to clean data and sometimes transform it.
    - The consequences of bad data for the model.
    - Data understanding is iterative; you learn more about your data the more you study it.

### **From Modeling to Evaluation**

- **Modeling**
    - Concepts
        
        ![Untitled](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/Untitled%2029.png)
        
        ![Untitled](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/Untitled%2030.png)
        
        ![Untitled](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/Untitled%2031.png)
        
        - Once modeled the data, model evaluation, deployment, and feedback loop ensure the answer is near and relevant
    - Case Study
        - Tuning the parameters to improve the model
        
        ![Untitled](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/Untitled%2032.png)
        
        - Upcoming question: How could the accuracy of the model be improved in predicting the yes outcome?
        
        ![Untitled](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/Untitled%2033.png)
        
        When a true, non-readmission is misclassified, and action is taken to reduce that patient's risk, the cost of that error is the wasted intervention. A statistician calls this a **type I error**, or a **false-positive**. 
        
        But when a true readmission is misclassified, and no action is taken to reduce that risk, then the cost of that error is the readmission and all its attended costs, plus the trauma to the patient. This is a **type II error**, ****or a **false-negative**.
        
        ![Untitled](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/Untitled%2034.png)
        
        - Problem: the large number of false-positives
        
        ![Untitled](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/Untitled%2035.png)
        
- **Evaluation**
    
    ![Untitled](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/Untitled%2036.png)
    
    - Model evaluation could have two phases:
        
        ![Untitled](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/Untitled%2037.png)
        
        1. Diagnostic measures
            
            Use to ensure the model is working as intended
            
            - (Upper left on Fig) E.g. if the model is a predictive mode, a decision tree could be used to evaluate if the answer the model can output, is aligned to the initial design
            - (Lower left on Fig) E.g. if the model is descriptive model, one in which relationships are being assessed, then testing set with knowhow can be applied, and the model can be refined as needed.
        2. Statistical significance testing
            
            This type of evaluation can be applied to the model to ensure that the data is being properly handled and interpreted within the model.
            
        - Case Study - Applying the concepts
            
            ![Untitled](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/Untitled%2038.png)
            
            ![Untitled](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/Untitled%2039.png)
            
            Problem: How could we determine which model is optimal?
            
            ![Untitled](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/Untitled%2040.png)
            
            By using ROC curve could solve the optmized problem
            
            Optimized model at the maximum separation as well as the distance between red and blue curves.
            
            The model 3, which has misclassification cost of 4-to-1, is the best of 4 models.
            
            - ROC curves is used to determine the optimal classification model (binary classification model)
            
            ![Untitled](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/Untitled%2041.png)
            
- Lab
    - [ ]  Done?
    
    [DS0103EN-Exercise-From-Modeling-to-Evaluation.ipynb](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/DS0103EN-Exercise-From-Modeling-to-Evaluation.ipynb)
    
- Lesson Summary
    
    In this lesson, you have learned:
    
    - The difference between descriptive and predictive models.
    - The role of training sets and test sets.
    - The importance of asking if the question has been answered.
    - Why diagnostic measures tools are needed.
    - The purpose of statistical significance tests.
    - That modeling and evaluation are iterative processes.

# Week03 - From Deployment to Feedback

## Pre

### **Learning Objectives**

---

- Describe the deployment and feedback phases of the data science methodology.
- Judge when a model is ready to deploy.
- Devise a plan to elicit feedback from stakeholders involved in the data analysis process.
- Examine how feedback helps to refine a model.
- Assess the performance and impact of a data model.
- Explain why deployment and feedback should be an iterative process.
- Devise a business problem to be solved with data related to either email, hospitals, or credit cards.
- Demonstrate your understanding of data science methodology by applying it to a given problem. Construct responses that address each phase of the CRISP-DM based on a chosen business problem.
- Evaluate your peers’ final projects using the given rubric. Provide constructive feedback and offer ideas and suggestions that fellow learners can apply right away.

## Deployment

![Untitled](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/Untitled%2042.png)

- Case Study
    
    ![Untitled](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/Untitled%2043.png)
    
    ![Untitled](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/Untitled%2044.png)
    
    ![Untitled](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/Untitled%2045.png)
    
    ![Untitled](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/Untitled%2046.png)
    
    ![Untitled](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/Untitled%2047.png)
    
    ![Untitled](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/Untitled%2048.png)
    

## Feedback

![Untitled](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/Untitled%2049.png)

- Case Study
    
    ![Untitled](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/Untitled%2050.png)
    
    After the deployment and feedback stages, the feedback of intervention program on re-admission rates will be reviewed after the first year of its implementation 
    
    ![Untitled](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/Untitled%2051.png)
    
    ![Untitled](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/Untitled%2052.png)
    

## Course Overall Summary

![Untitled](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/Untitled%2053.png)

![Untitled](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/Untitled%2054.png)

![Untitled](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/Untitled%2055.png)

![Untitled](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/Untitled%2056.png)

![Untitled](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/Untitled%2057.png)

![Untitled](3%20Data%20Science%20Methodology%205977e32ec6444c92bad4579938ea7064/Untitled%2058.png)

## Lesson Summary

In this lesson, you have learned:

- The importance of stakeholder input.
- To consider the scale of deployment.
- The importance of incorporating feedback to refine the model.
- The refined model must be redeployed.
- This process should be repeated as often as necessary.