# 2. Tools for Data Science

---

# Week01 - Data Scientist's Toolkit

## **Languages of Data Science**

## ****Data Science Tools****

### **Data Science Tools - Open Sources**

![Untitled](2%20Tools%20for%20Data%20Science%20d51c4d90a2cb44d2964211d2dc965f0c/Untitled.png)

- Data management
    - SQL:
        - MySQL
        - PostgreSQL
    - NoSQL:
        - MongoDB
        - Apache CouchDB
        - Apache Cassandra
    - File-based tool:
        - Hadoop
    - System or could file systems:
        - Ceph
    - Text data (or create a search index)
        - Elasticsearch
- Data Integration and Transformation (in the classics data warehousing)
    - ETL (Extra, Transform, Load) = ELT (Extra, Load, Transform)
    - Rename this stage as: **Data refinery and cleaning**
    - Tools:
        - Apache Airflow
        - Kobeflow
        - Apache Kafka
        - Apache Nifi
        - Apache Spark SQL
            - Using ANSI SQL
            - Multiple computer clusters (up to 1000 nodes)
        - NodeRED
            - Could use at Raspberry Pi
- Data Visualization
    - Tools:
        - HUE
            - could create visualizations from SQL queries
        - Kibana
            - data exploration and visualization web application (limited to Elasticsearch)
        - 
            - data exploration and visualization web application
- Model Deployment
    - Once built a machine learning model, we should make the model consumable by other developers and turn it into API
    - Tools:
        - Apache PredictionIO
            - Only for Apache Spark ML models
        - SELDON
            - Includes: TensorFlow, SparkML, R, scikit-learn
            - Could run top up of Kubernetes and Redhat OpenShift
        - mleap
            - TesorFlow service, TensorFlow Lite, TensorFlow.JS
- Model Monitoring and Assessment
    - Once we deployed a machine learning model, we need to keep track of its prediction performance as new data for maintaining the outdated models
    - Tools:
        - ModelDB
            - A machine model metadatabase where information of the models are stored and can be queried
            - A system to manage ML models
            - For Apache Spark ML Pipelines and scikit-learn
        - Prometheus
        - IBM Research Trusted AI…
- Code Asset Management
    - Version management or version control
    - Also know as data governance or data lineage
    - Tools:
        - git
        - GitHub
        - GitLab
            - Could host and manage by ourself
        - Bitbucket
    - Tools for version and annotation with metadata
        - Apache Atlas
        - ODPi EGERIA
            - Linux foundation
        - Kylo
- Development Environment
    - Jupyter
        - Documentation, Code, Output from the code, Shell commands, Visualization in one single document
    - Jupyter Lab
        - Next generation of Jupyter notebooks
    - Apache Zeppelin
    - R studio
    - Spyder
- Execution Environment
    - Apache Spark
        - Sometimes data doesn’t fit into a single computer’s storage or maintain memory capacity. → cluster execution environment come in to play a role
        - Well-known cluster-computering framework
        - Linear scalability → double the number of servers, at the same time, almost double the performance
    - Apache Flink
        - The batch from Apache Spark, which could capable of processing huge amount of data file by file
        - Stream processing image → focus on real-time data streams
    - riselab Ray
        - Large scale deep learning data training
    - Fully Integrated Visual Tools
        - Which includes “Data Integration and transformation”, “Data visualization”, “Model Building”
        - Tools:
            - KNIME - originated at University of Konstanz
                - drag-and-drop capabilities
                - Built-in visualization capabilities
                - extend from R or python and could extend to Spark as well
            - Orange

### Data Science Tools - Commercial Tools (ETL tools)

![Untitled](2%20Tools%20for%20Data%20Science%20d51c4d90a2cb44d2964211d2dc965f0c/Untitled.png)

- Data management
    
    ![Untitled](2%20Tools%20for%20Data%20Science%20d51c4d90a2cb44d2964211d2dc965f0c/Untitled%201.png)
    
- Data Integration and Transformation (in the classics data warehousing)
    
    ![Untitled](2%20Tools%20for%20Data%20Science%20d51c4d90a2cb44d2964211d2dc965f0c/Untitled%202.png)
    
- Data Visualization
    - create a dashbroad
    
    ![Untitled](2%20Tools%20for%20Data%20Science%20d51c4d90a2cb44d2964211d2dc965f0c/Untitled%203.png)
    
- Model Building
    
    ![Untitled](2%20Tools%20for%20Data%20Science%20d51c4d90a2cb44d2964211d2dc965f0c/Untitled%204.png)
    
- Model Deployment
    
    ![Untitled](2%20Tools%20for%20Data%20Science%20d51c4d90a2cb44d2964211d2dc965f0c/Untitled%205.png)
    
- Model Monitoring and Assessment
    - No commercial software is avalable now, only open sources
- Code Asset Management
    - No commercial software is avalable now, only open sources
    - Git or GitHub is effective standard
- Data Asset Management
    - Also know as data governance or data lineage
    
    ![Untitled](2%20Tools%20for%20Data%20Science%20d51c4d90a2cb44d2964211d2dc965f0c/Untitled%206.png)
    
    The IBM InfoSphere Information Governance Catalog covers functions like data dictionary, which facilitates discovery of data assets. Each data asset is assigned to a data steward -- the data owner. The data owner is responsible for that data asset and can be contacted. Data lineage is also covered; this enables a user to track back through the transformation steps followed in creating the data assets. The data lineage also includes a reference to the actual source data. Rules and policies can be added to reflect complex regulatory and business requirements for data privacy and retention.
    
- Development Environments
    
    ![Untitled](2%20Tools%20for%20Data%20Science%20d51c4d90a2cb44d2964211d2dc965f0c/Untitled%207.png)
    
    - Fully intergrated Visual Tools:
        
        ![Untitled](2%20Tools%20for%20Data%20Science%20d51c4d90a2cb44d2964211d2dc965f0c/Untitled%208.png)
        
- Execution Environment
    - 

### Cloud Based Tools

Conventional Architecture:

![Untitled](2%20Tools%20for%20Data%20Science%20d51c4d90a2cb44d2964211d2dc965f0c/Untitled.png)

For cloud based: 

![Untitled](2%20Tools%20for%20Data%20Science%20d51c4d90a2cb44d2964211d2dc965f0c/Untitled%209.png)

- Fully Integrated Visual Tools and Platforms
    - Watson Studio + Watson OpenScale
        
        [https://www.notion.so](https://www.notion.so)
        
        - Watson Studio, together with Watson OpenScale, covers the complete development life cycle for all data science, machine learning, and AI tasks.
    - Azure - Microsoft
        
        ![Untitled](2%20Tools%20for%20Data%20Science%20d51c4d90a2cb44d2964211d2dc965f0c/Untitled%2010.png)
        
        - Microsoft Azure Machine Learning. This is also a fully cloud-hosted offering supporting the complete development life cycle of all data science, machine learning, and AI tasks.
    - H2O Driverless AI
        
        SaaS: Software as a Service (another one Paas: Platform as a Service)
        
        ![Untitled](2%20Tools%20for%20Data%20Science%20d51c4d90a2cb44d2964211d2dc965f0c/Untitled%2011.png)
        
- Data management
    
    ![Untitled](2%20Tools%20for%20Data%20Science%20d51c4d90a2cb44d2964211d2dc965f0c/Untitled%2012.png)
    
- Data Integration and Transformation (in the classics data warehousing)
    
    ![Untitled](2%20Tools%20for%20Data%20Science%20d51c4d90a2cb44d2964211d2dc965f0c/Untitled%2013.png)
    
- Data Visualization
    
    ![Untitled](2%20Tools%20for%20Data%20Science%20d51c4d90a2cb44d2964211d2dc965f0c/Untitled%2014.png)
    
- Model Building
    
    ![Untitled](2%20Tools%20for%20Data%20Science%20d51c4d90a2cb44d2964211d2dc965f0c/Untitled%2015.png)
    
- Model Deployment
    
    ![Untitled](2%20Tools%20for%20Data%20Science%20d51c4d90a2cb44d2964211d2dc965f0c/Untitled%2016.png)
    
- Model Monitoring and Assessment
    
    ![Untitled](2%20Tools%20for%20Data%20Science%20d51c4d90a2cb44d2964211d2dc965f0c/Untitled%2017.png)
    
    - Watson Studio + Watson OpenScale could cover the green parts in the follwoing figures
    
    ![Untitled](2%20Tools%20for%20Data%20Science%20d51c4d90a2cb44d2964211d2dc965f0c/Untitled%2018.png)
    

## **Packages, APIs, Data Sets and Models**

### Libraries for data science

- Libraries are a collection of functions and methods that enable you to perform a wide variety of actions without writing the code yourself.

![Untitled](2%20Tools%20for%20Data%20Science%20d51c4d90a2cb44d2964211d2dc965f0c/Untitled%2019.png)

- Data visualization methods are a great way to communicate with others and show the meaningful results of analysis.

![Untitled](2%20Tools%20for%20Data%20Science%20d51c4d90a2cb44d2964211d2dc965f0c/Untitled%2020.png)

- For machine learning, the Scikit-learn library contains tools for statistical modeling, including regression, classification, clustering and others. It is built on NumPy, SciPy, and matplotlib, and it’s relatively simple to get started.

![Untitled](2%20Tools%20for%20Data%20Science%20d51c4d90a2cb44d2964211d2dc965f0c/Untitled%2021.png)

![Untitled](2%20Tools%20for%20Data%20Science%20d51c4d90a2cb44d2964211d2dc965f0c/Untitled%2022.png)

- Apache Spark is a general-purpose cluster-computing framework that enables you to process data using compute clusters. This means that you process data in parallel, using multiple computers simultaneously. The Spark library has similar functionality as Pandas Numpy Scikit-learn.
    
    ![Untitled](2%20Tools%20for%20Data%20Science%20d51c4d90a2cb44d2964211d2dc965f0c/Untitled%2023.png)
    
- Apache Spark data processing jobs can use Python R Scala, or SQL

![Untitled](2%20Tools%20for%20Data%20Science%20d51c4d90a2cb44d2964211d2dc965f0c/Untitled%2024.png)

- Scala-library

![Untitled](2%20Tools%20for%20Data%20Science%20d51c4d90a2cb44d2964211d2dc965f0c/Untitled%2025.png)

- R has built-in functionality for machine learning and data visualization

![Untitled](2%20Tools%20for%20Data%20Science%20d51c4d90a2cb44d2964211d2dc965f0c/Untitled%2026.png)

### Application Programming Interface (API)

- An API lets two pieces of software talk to each other.
    
    ![Screen Shot 2022-09-29 at 11.16.16 AM.png](2%20Tools%20for%20Data%20Science%20d51c4d90a2cb44d2964211d2dc965f0c/Screen_Shot_2022-09-29_at_11.16.16_AM.png)
    
- Pandas’ API

![Untitled](2%20Tools%20for%20Data%20Science%20d51c4d90a2cb44d2964211d2dc965f0c/Untitled%2027.png)

- REST APIs
    - They enable you to communicate using the internet, taking advantage of storage, greater data access, artificial intelligence algorithms, and many other resources.
    - REpresentational State Transfer APIs
    
    ![Untitled](2%20Tools%20for%20Data%20Science%20d51c4d90a2cb44d2964211d2dc965f0c/Untitled%2028.png)
    
    - Procedure
    
    ![Untitled](2%20Tools%20for%20Data%20Science%20d51c4d90a2cb44d2964211d2dc965f0c/Untitled%2029.png)
    

### Data Sets - Powering Data Science

- Where to find the open data

![Untitled](2%20Tools%20for%20Data%20Science%20d51c4d90a2cb44d2964211d2dc965f0c/Untitled%2030.png)

- Community Data License Agreement
    - CDLA-Sharing:
        - The license stipulates that if you publish your modified version of the data you must do so under the same license terms as the original data.
    - CDLA-Permissive:
        - do not required to share changes to the data
    - Example:
        - You are building a model that performs a prediction. If you are training the model using CDLA-licensed data sets, you are under no obligation to share the model, or to share it under a specific license if you do choose to share it.

![Untitled](2%20Tools%20for%20Data%20Science%20d51c4d90a2cb44d2964211d2dc965f0c/Untitled%2031.png)

### Sharing Enterprise Data - Data Asset eXchange

- IBM Data Asset eXchange - DAX

### Machine Learning Models

![Untitled](2%20Tools%20for%20Data%20Science%20d51c4d90a2cb44d2964211d2dc965f0c/Untitled%2032.png)

- Machine Learning
    - Supervised Learning
        - Supervised learning is used to solve regression and classification problems
    
    ![Untitled](2%20Tools%20for%20Data%20Science%20d51c4d90a2cb44d2964211d2dc965f0c/Untitled%2033.png)
    
    - Unsupervised Learning
        - clustering
            - Clustering models are used to divide each record of a data set into one of a small number of similar groups.
            - Example:
                - An example of a clustering model could be providing purchase recommendations for an e-commerce store based on past shopping behavior and the content of a shopping basket.
        - anomaly detection
            - Anomaly detection identifies outliers in a data set, such as fraudulent credit card transactions or suspicious online log-in attempts.
    
    ![Untitled](2%20Tools%20for%20Data%20Science%20d51c4d90a2cb44d2964211d2dc965f0c/Untitled%2034.png)
    
    - Reinforcement learning
        - loosely based on the way human beings and other organisms learn
        - A reinforcement learning model learns the best set of actions to take, given its current environment, in order to get the most reward over time.
        - Example:
            - Think about a mouse in a maze. If the mouse gets to the end of the maze it gets a piece of cheese. This is the “reward” for completing a task. The mouse learns – through trial and error – how to get through the maze to get as much cheese as it can.
    
    ![Untitled](2%20Tools%20for%20Data%20Science%20d51c4d90a2cb44d2964211d2dc965f0c/Untitled%2035.png)
    
- Deep Learning
    - Try to loosely emulate how humans brain works
    
    ![Untitled](2%20Tools%20for%20Data%20Science%20d51c4d90a2cb44d2964211d2dc965f0c/Untitled%2036.png)
    
    ![Untitled](2%20Tools%20for%20Data%20Science%20d51c4d90a2cb44d2964211d2dc965f0c/Untitled%2037.png)
    
    - Example of using deep learning model to solve problem
        
        ![Untitled](2%20Tools%20for%20Data%20Science%20d51c4d90a2cb44d2964211d2dc965f0c/Untitled%2038.png)
        

### The Model Asset Exchange

![Untitled](2%20Tools%20for%20Data%20Science%20d51c4d90a2cb44d2964211d2dc965f0c/Untitled%2039.png)

- MAX is built by Docker image

![Untitled](2%20Tools%20for%20Data%20Science%20d51c4d90a2cb44d2964211d2dc965f0c/Untitled%2040.png)

# Week02 - Open Source Tools

## Jupyter Notebook and JupyterLab

- A Jupyter notebook is a browser-based application that allows you to create and share documents that contain code, equations, visualizations, narrative text links, and so much more.

![Untitled](2%20Tools%20for%20Data%20Science%20d51c4d90a2cb44d2964211d2dc965f0c/Untitled%2041.png)

- Jupyter stands for:
    - **Ju**lia, **Py**thon, **R**
    - but nowadays it supports: Java, Scala, MATLAB, Octave, Ruby, JS

---

- Jupyter Lab is a browser-based application that allows you to access multiple Jupyter Notebook files as well as other code and data files.

---

- What is a kernel?
    - In aA notebook kernel is a computational engine that executes the code contained in a Notebook file.

---

- Markdown Cheatsheet
    
    [Markdown Cheatsheet · adam-p/markdown-here Wiki](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
    
- Recommendations
    - First you start with exploratory data analysis, so this notebook is highly recommended to have a look at:
        
        [Notebook on nbviewer](https://nbviewer.jupyter.org/github/Tanu-N-Prabhu/Python/blob/master/Exploratory_data_Analysis.ipynb?utm_medium=Exinfluencer&utm_source=Exinfluencer&utm_content=000026UJ&utm_term=10006555&utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMDeveloperSkillsNetworkDS0105ENSkillsNetwork20083975-2022-01-01)
        
    - For data integration / cleansing at a smaller scale, the python library *pandas* is often used. Please have a look at this notebook:
        
        [Data Cleaning with Python using Pandas Library.](https://towardsdatascience.com/data-cleaning-with-python-using-pandas-library-c6f4a68ea8eb?utm_medium=Exinfluencer&utm_source=Exinfluencer&utm_content=000026UJ&utm_term=10006555&utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMDeveloperSkillsNetworkDS0105ENSkillsNetwork20083975-2022-01-01)
        
    - If you want to already experience what clustering is, have a look at this:
        
        [Notebook on nbviewer](https://nbviewer.jupyter.org/github/temporaer/tutorial_ml_gkbionics/blob/master/2%20-%20KMeans.ipynb?utm_medium=Exinfluencer&utm_source=Exinfluencer&utm_content=000026UJ&utm_term=10006555&utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMDeveloperSkillsNetworkDS0105ENSkillsNetwork20083975-2022-01-01)
        
    - And finally, if you want to go for a more in-depth notebook on the *iris* dataset have a look here:
        
        [Iris Dataset - Exploratory Data Analysis](https://www.kaggle.com/lalitharajesh/iris-dataset-exploratory-data-analysis?utm_medium=Exinfluencer&utm_source=Exinfluencer&utm_content=000026UJ&utm_term=10006555&utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMDeveloperSkillsNetworkDS0105ENSkillsNetwork20083975-2022-01-01)
        

## RStudio IDE

## GitHub

- Notes
    - Recommendations Materials
        
        [Set up Git - GitHub Docs](https://docs.github.com/en/get-started/quickstart/set-up-git)
        
    - Why we need to create a “branch”
    
    ![Untitled](2%20Tools%20for%20Data%20Science%20d51c4d90a2cb44d2964211d2dc965f0c/Untitled%2042.png)
    
    - Pull Request (PR)
    
    ![Untitled](2%20Tools%20for%20Data%20Science%20d51c4d90a2cb44d2964211d2dc965f0c/Untitled%2043.png)
    
- Git Command - setting key
    
    ## **設定金鑰步驟**
    
    ### **Step 1 產生金鑰**
    
    使用以下指令產生金鑰：
    
    ```
    ssh-keygen
    ```
    
    後面的選項一律按 Enter 同意；產生的金鑰（**id_rsa** 和 **id_rsa.pub**）會放在 ~/.ssh 路徑底下。
    
    ### **Step 2 上傳金鑰（id_rsa.pub）**
    
    來到 GitHub，並打開右上角個人圖示的選單，選擇底下的 **Settings** 選項。
    
    ![https://i0.wp.com/clay-atlas.com/wp-content/uploads/2021/05/Screenshot-from-2021-05-22-21-06-26.png?resize=269%2C505&ssl=1](https://i0.wp.com/clay-atlas.com/wp-content/uploads/2021/05/Screenshot-from-2021-05-22-21-06-26.png?resize=269%2C505&ssl=1)
    
    進入後，再選擇左側選項中的 **SSH and GPG keys** 選項。
    
    ![https://i0.wp.com/clay-atlas.com/wp-content/uploads/2021/05/Screenshot-from-2021-05-22-21-08-47.png?resize=1024%2C675&ssl=1](https://i0.wp.com/clay-atlas.com/wp-content/uploads/2021/05/Screenshot-from-2021-05-22-21-08-47.png?resize=1024%2C675&ssl=1)
    
    選擇添加新的 **SSH keys**。
    
    ![https://i0.wp.com/clay-atlas.com/wp-content/uploads/2021/05/Screenshot-from-2021-05-22-21-09-21.png?resize=758%2C119&ssl=1](https://i0.wp.com/clay-atlas.com/wp-content/uploads/2021/05/Screenshot-from-2021-05-22-21-09-21.png?resize=758%2C119&ssl=1)
    
    **Title** 可以自己設定一個好記的名稱，底下的 **Key** 則要完整填入 **id_rsa.pub** 中的內容，多一個空格也不行。
    
    ![https://i0.wp.com/clay-atlas.com/wp-content/uploads/2021/05/Screenshot-from-2021-05-22-21-10-41.png?resize=783%2C427&ssl=1](https://i0.wp.com/clay-atlas.com/wp-content/uploads/2021/05/Screenshot-from-2021-05-22-21-10-41.png?resize=783%2C427&ssl=1)
    
    ### **Step 3 設定 GitHub 個人帳戶訊息**
    
    我老是忘記這個步驟，順帶紀錄。將自己現在使用的裝置進行 git 設定。
    
    - Error: **[push declined due to email privacy restrictions](https://stackoverflow.com/questions/43378060/meaning-of-the-github-message-push-declined-due-to-email-privacy-restrictions)**
        
        The remote repository has been configured to disallow you pushing a commit that would reveal your personal e-mail address. For example in GitHub you have checked the *[Block command line pushes that expose my email](https://github.com/settings/emails)* checkbox to [enable this](https://github.com/blog/2346-private-emails-now-more-private).
        
        ![https://i.stack.imgur.com/qUWWQ.png](https://i.stack.imgur.com/qUWWQ.png)
        
        While you can of course uncheck that setting, it will expose your private e-mail address to everyone in the world, as author information is readable by anyone with access to your repository.
        
        Instead, do this:
        
        1. You can see your personal e-mail address, which is used by default for your commits in Git:
            
            ```
            git config --global user.email
            
            ```
            
        2. Find your [GitHub noreply address](https://help.github.com/articles/setting-your-email-in-git/) in your GitHub's [Personal Settings → Emails](https://github.com/settings/emails). It's mentioned in the description of the *Keep my email address private* checkbox. Usually, it starts with a unique identifier, plus your username:
            
            ```
            {ID}+{username}@users.noreply.github.com
            
            ```
            
            ![https://i.stack.imgur.com/pFiwC.png](https://i.stack.imgur.com/pFiwC.png)
            
        3. Change the global user e-mail address setting to be your GitHub noreply address:
            
            ```
            git config --global user.email {ID}+{username}@users.noreply.github.com
            
            ```
            
        4. Reset the author information on your last commit:
            
            ```
            git commit --amend --reset-author
            
            ```
            
            If you have multiple commits with your private e-mail address, see [this answer](https://stackoverflow.com/a/25815116/146622).
            
        5. Now you can push the commit with the noreply e-mail address, and future commits will have the noreply e-mail address as well.
            
            ```
            git push
            ```
            
    
    ```
    git config --global user.email "you@example.com"
    git config --global user.name "Your Name"
    ```
    
- **Working with GitHub on local machine**
    
    **BASH Installation**
    
    *For Windows:*
    
    [GitBash Installation](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DS0105EN-SkillsNetwork/labs/Module2/GitBash_Install.md.html?utm_medium=Exinfluencer&utm_source=Exinfluencer&utm_content=000026UJ&utm_term=10006555&utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMDeveloperSkillsNetworkDS0105ENSkillsNetwork20083975-2022-01-01)
    
    *For Linux/Unix:*
    
    For Linux systems installing Git is easy. If you are using a Debian-based distribution like Ubuntu, you can use apt install:
    
    $ sudo apt install git-all
    
    For Fedora, RHEL or CentOS, you can use:
    
    $ sudo dnf install git-all
    
    *For Mac:*
    
    Open the Terminal
    
    Install homebrew if you don't already have it, then:
    
    $ brew install git
    
    **SSH Key generation**
    
    [Generate SSH Key](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DS0105EN-SkillsNetwork/labs/Module2/GitHub_SSHKey.md.html?utm_medium=Exinfluencer&utm_source=Exinfluencer&utm_content=000026UJ&utm_term=10006555&utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMDeveloperSkillsNetworkDS0105ENSkillsNetwork20083975-2022-01-01)
    
- ****Adding SSH Key to GitHub****
    
    ork, use `cat ~/.ssh/id_rsa.pub` on command line and the copy the output.
    
    Step 2: Now, Open GitHub and go to `Setting` (Click on the arrow)
    
    ![https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DS0105EN-SkillsNetwork/labs/Module2/images/settings.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DS0105EN-SkillsNetwork/labs/Module2/images/settings.png)
    
    Step 3: Under Personal settings, select `SSH and GPG keys`, as shown below:
    
    ![https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DS0105EN-SkillsNetwork/labs/Module2/images/SSHKey_option_new.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DS0105EN-SkillsNetwork/labs/Module2/images/SSHKey_option_new.png)
    
    Step 4: Click the button to add a `New SSH key`.
    
    ![https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DS0105EN-SkillsNetwork/labs/Module2/images/AddNewSSH.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DS0105EN-SkillsNetwork/labs/Module2/images/AddNewSSH.png)
    
    Step 5: Provide the title. Then select the Key field, and press Ctrl-v to paste the key from the clipboard buffer. The pasted key should have **your email address** at the end, as shown below:
    
    ![https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DS0105EN-SkillsNetwork/labs/Module2/images/add_ssh_keytoaccount_new.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DS0105EN-SkillsNetwork/labs/Module2/images/add_ssh_keytoaccount_new.png)
    
    and click `Add SSH Key`.
    
    Now, the SSH key is added to your account.
    
    ## **Summary**
    
    In this document, you have learned how to add SSH key to GitHub.
    
- **Creating Repository in GitHub**
    
    ## **Creating Repository in GitHub**
    
    **Objectives of this Exercise**
    
    - To create a repository in GitHub with README.md
    - To create a repository in GitHub without README.md
    
    *Note: These instructions works on BASH terminal on Windows & Mac terminals.*
    
    ## **Exercise**
    
    1. Create a new repository (it’s a container where all stuff goes) using the + sign as shown below:
    
    ![https://user-images.githubusercontent.com/25001852/86895774-991bb480-c122-11ea-9e0a-0e6ab95c397b.png](https://user-images.githubusercontent.com/25001852/86895774-991bb480-c122-11ea-9e0a-0e6ab95c397b.png)
    
    1. Provide the necessary details like repository name. Select repository as Public and initialize the READMD. Click ‘Create’.
    
    ![https://user-images.githubusercontent.com/25001852/86910859-f3734000-c137-11ea-89cd-763ad102f971.png](https://user-images.githubusercontent.com/25001852/86910859-f3734000-c137-11ea-89cd-763ad102f971.png)
    
    Now, your repository is created, and it looks as:
    
    ![https://user-images.githubusercontent.com/25001852/86910903-0b4ac400-c138-11ea-89f8-4a39e7d3e459.png](https://user-images.githubusercontent.com/25001852/86910903-0b4ac400-c138-11ea-89f8-4a39e7d3e459.png)
    
    1. To download the repository, we have option'Download Zip' in 'Code'. Also, there are two options to copy repository locally using ‘SSH’ and ‘HTTPS’
    
    ![https://user-images.githubusercontent.com/25001852/86896805-2e6b7880-c124-11ea-9c3e-fc7b43a47cc9.png](https://user-images.githubusercontent.com/25001852/86896805-2e6b7880-c124-11ea-9c3e-fc7b43a47cc9.png)
    
    ![https://user-images.githubusercontent.com/25001852/86896922-5d81ea00-c124-11ea-852a-d0dc5d9d135a.png](https://user-images.githubusercontent.com/25001852/86896922-5d81ea00-c124-11ea-852a-d0dc5d9d135a.png)
    
    1. Copy the SSHRepositoryLink on to your clipboard.
    2. Open the command prompt or terminal to use the GitHub commands:
        - To change the directory simply use:
        
        `cd <name of the directory you want to change to>`
        
        - To go to the folder “Downloads” use: `cd Downloads`
    3. Use the SSH repository link from out GitHub Repository and clone it to your local system as follows:
    
    `git clone pastesshrepositorylinkhere`
    
    ![https://user-images.githubusercontent.com/25001852/86911345-ce330180-c138-11ea-9f97-966489c07c72.png](https://user-images.githubusercontent.com/25001852/86911345-ce330180-c138-11ea-9f97-966489c07c72.png)
    
    1. Now, the folder is copied to my ‘Downloads’. Just check the ‘Downloads’ have you got the folder demo.
        - To check my folder, enter the folder using cd command again as:
        
        `cd demo`
        
    2. Get the list of the files in the folder demo, use: For Windows: `dir` For Mac: `ls`
    
    ![https://user-images.githubusercontent.com/25001852/86911459-f9b5ec00-c138-11ea-8d45-7da44bbc20c1.png](https://user-images.githubusercontent.com/25001852/86911459-f9b5ec00-c138-11ea-8d45-7da44bbc20c1.png)
    
    1. To view the content of the file: For Windows: `type README.md` For Mac: `cat README.md`
    2. To open a README.md file: For Windows: `notepad README.md` For Mac: `open README.md`
    3. To create a new file: For Windows: `notepad test.txt` For Mac: `vi test.txt`
    4. Add to the repository: For Windows/Mac: `git add test.txt`
        - Check the status of the file using:
        
        `git status`
        
    
    ![https://user-images.githubusercontent.com/25001852/86912050-ece5c800-c139-11ea-8046-99f987f9d644.png](https://user-images.githubusercontent.com/25001852/86912050-ece5c800-c139-11ea-8046-99f987f9d644.png)
    
    1. Commit the changes in the repository using:
    
    `git commit -m “write message here”`
    
    ![https://user-images.githubusercontent.com/25001852/86912336-6b426a00-c13a-11ea-8652-3df5246b5793.png](https://user-images.githubusercontent.com/25001852/86912336-6b426a00-c13a-11ea-8652-3df5246b5793.png)
    
    1. Push the file to remote repository using:
    
    `git push`
    
    ![https://user-images.githubusercontent.com/25001852/86912378-801efd80-c13a-11ea-8ab2-ffafb2abbb02.png](https://user-images.githubusercontent.com/25001852/86912378-801efd80-c13a-11ea-8ab2-ffafb2abbb02.png)
    
    Now, this make the changes in my GitHub repository
    
    ![https://user-images.githubusercontent.com/25001852/86912441-9fb62600-c13a-11ea-85ed-df150393a285.png](https://user-images.githubusercontent.com/25001852/86912441-9fb62600-c13a-11ea-85ed-df150393a285.png)
    
    ## **Create a repository now without README.md file**
    
    ![https://user-images.githubusercontent.com/25001852/86912607-eb68cf80-c13a-11ea-8a51-2569f53ccdd7.png](https://user-images.githubusercontent.com/25001852/86912607-eb68cf80-c13a-11ea-8a51-2569f53ccdd7.png)
    
    1. Copy the SSHRepositoryLink on to your clipboard as did before
    2. To come out from the demo folder first use
    
    `cd ..`
    
    1. To make a directory in download folder:
    
    `mkdir demo1` `cd demo1`
    
    ![https://user-images.githubusercontent.com/25001852/86913896-f886be00-c13c-11ea-8293-11d987521b2e.png](https://user-images.githubusercontent.com/25001852/86913896-f886be00-c13c-11ea-8293-11d987521b2e.png)
    
    1. To create a readmd file use
    
    `echo "# demo1" >> README.md`
    
    1. Initialize the directory
    
    `git init`
    
    1. Create and add a README.md file. You can use a normal text editor depending on which OS you are using.
    
    `git add README.md`
    
    1. Check the status of the file
    
    `git status`
    
    1. Commit the changes
    
    `git commit -m "first commit"`
    
    1. Add the origin where we have to push the file. This is the SSHRepositoryLink you copied when you created the repository.
    
    `git remote add origin git@github.com:mskill/demo1.git`
    
    1. Push the file
    
    `git push -u origin master`
    
    ![https://user-images.githubusercontent.com/25001852/86914009-31269780-c13d-11ea-8519-76d4103be861.png](https://user-images.githubusercontent.com/25001852/86914009-31269780-c13d-11ea-8519-76d4103be861.png)
    
    Now, the README.md file is created in our repository
    
    ![https://user-images.githubusercontent.com/25001852/86914078-51565680-c13d-11ea-9d36-752638d1725e.png](https://user-images.githubusercontent.com/25001852/86914078-51565680-c13d-11ea-9d36-752638d1725e.png)
    
    ## **Author(s)**
    
- ****Add file to Repository in GitHub****
    
    **Objective for Exercise**
    
    - To add file to repository on GitHub
    - To add file to repository on GitHub through command line
    
    *Note: These instructions works on BASH terminal on Windows & Mac terminals.*
    
    Click 'Add file' to add a file
    
    ![https://user-images.githubusercontent.com/25001852/86914757-726b7700-c13e-11ea-8411-dbe00b06171c.png](https://user-images.githubusercontent.com/25001852/86914757-726b7700-c13e-11ea-8411-dbe00b06171c.png)
    
    Provide the file name and add a description to that file. To commit the changes in the repository, click ‘Commit New File’
    
    ![https://user-images.githubusercontent.com/25001852/86914831-9464f980-c13e-11ea-869e-71569f13011f.png](https://user-images.githubusercontent.com/25001852/86914831-9464f980-c13e-11ea-869e-71569f13011f.png)
    
    ![https://user-images.githubusercontent.com/25001852/86914872-a6df3300-c13e-11ea-8c0f-b71f95601af2.png](https://user-images.githubusercontent.com/25001852/86914872-a6df3300-c13e-11ea-8c0f-b71f95601af2.png)
    
    Adding a file remotely will not be there in the local directory. Check the files using `dir`
    
    ![https://user-images.githubusercontent.com/25001852/86915095-04737f80-c13f-11ea-944a-2c7cf9f06e8e.png](https://user-images.githubusercontent.com/25001852/86915095-04737f80-c13f-11ea-944a-2c7cf9f06e8e.png)
    
    As per the screenshot above, there is 1 file in the repository.
    
    To pull the file that is added in remote repository to local repository, we use PULL command `git pull`
    
    ![https://user-images.githubusercontent.com/25001852/86915220-3b499580-c13f-11ea-9ca1-1a520fbd61cc.png](https://user-images.githubusercontent.com/25001852/86915220-3b499580-c13f-11ea-9ca1-1a520fbd61cc.png)
    
    After pull, if I check the local repository using dir, there are 2 files as shown:
    
    ![https://user-images.githubusercontent.com/25001852/86915357-7cda4080-c13f-11ea-8550-19deeacc42a9.png](https://user-images.githubusercontent.com/25001852/86915357-7cda4080-c13f-11ea-8550-19deeacc42a9.png)
    
    To add a branch in master branch `git branch branchname`
    
    Switch the branch `git checkout branchname`
    
    Adding a file in branch `echo "#content">> filename.txt`
    
    Then add the file and push the file. To create the branch remotely we have to use `git push --set-upstream origin branchname`
    
    ![https://user-images.githubusercontent.com/25001852/86916988-07bc3a80-c142-11ea-88c3-e395f9cfc9b3.png](https://user-images.githubusercontent.com/25001852/86916988-07bc3a80-c142-11ea-88c3-e395f9cfc9b3.png)
    
    Switch the branch again to the master using `git checkout master`
    
    Merge command to merge the branches `git merge mybranch`
    
    As the merge command is used the new create branch will be merged to the master branch and the file will be inserted to it. Previously, we have 2 file in the master, now there are 3 files. Make sure to push the files using
    
    ```
    git push
    ```
    
    ![https://user-images.githubusercontent.com/25001852/86917132-3e925080-c142-11ea-859b-1652369ddd8b.png](https://user-images.githubusercontent.com/25001852/86917132-3e925080-c142-11ea-859b-1652369ddd8b.png)
    
    Now, the file which is in the branch, is now in the master branch
    
    ![https://user-images.githubusercontent.com/25001852/86917264-68e40e00-c142-11ea-8f75-934002d6e1ab.png](https://user-images.githubusercontent.com/25001852/86917264-68e40e00-c142-11ea-8f75-934002d6e1ab.png)
    
- ****Fork and Pull****
    
    ## **Fork and Pull**
    
    **Objective for Exercise**
    
    - To fork a repository in GitHub
    - To make changes to the forked repository and commit the changes
    - To create pull requests
    
    *Note: These instructions works on BASH terminal on Windows & Mac terminals.*
    
    ## **How to fork a repository and commit the fork repository and create a pull request.**
    
    Open the link: [https://github.com/romeokienzler/TensorFlow/](https://github.com/romeokienzler/TensorFlow/)
    
    Click ‘Fork’ and copy the repository in your account.
    
    Copy the SSH Repository Link and clone it locally using:
    
    `git clone yoursshrepolink`
    
    ![https://user-images.githubusercontent.com/25001852/86918986-1eb05c00-c145-11ea-816f-56d3de31d92c.png](https://user-images.githubusercontent.com/25001852/86918986-1eb05c00-c145-11ea-816f-56d3de31d92c.png)
    
    Open and edit any file in the editor.
    
    After saving the file,
    
    `git add .`
    
    And commit the changes with the message:
    
    `git commit -m “message”`
    
    ![https://user-images.githubusercontent.com/25001852/86919047-3687e000-c145-11ea-87db-c7afe102eb5f.png](https://user-images.githubusercontent.com/25001852/86919047-3687e000-c145-11ea-87db-c7afe102eb5f.png)
    
    `git push` to make the changes in remote repository
    
    ![https://user-images.githubusercontent.com/25001852/86919111-57503580-c145-11ea-9918-c6a78271d181.png](https://user-images.githubusercontent.com/25001852/86919111-57503580-c145-11ea-9918-c6a78271d181.png)
    
    Check the repository, it is added
    
    ![https://user-images.githubusercontent.com/25001852/86919173-7353d700-c145-11ea-9457-79c422a76bd2.png](https://user-images.githubusercontent.com/25001852/86919173-7353d700-c145-11ea-9457-79c422a76bd2.png)
    
    Click ‘Compare’ to compare the changes.
    
    ![https://user-images.githubusercontent.com/25001852/86919301-a5fdcf80-c145-11ea-8657-176d3c9f7d46.png](https://user-images.githubusercontent.com/25001852/86919301-a5fdcf80-c145-11ea-8657-176d3c9f7d46.png)
    
    NOTE: This request will go to AUTHOR of the repository and if the changes looks good, only then the original repository can get the changes.
    
    ![https://user-images.githubusercontent.com/25001852/86919351-b9a93600-c145-11ea-8d69-ff15b68d73d9.png](https://user-images.githubusercontent.com/25001852/86919351-b9a93600-c145-11ea-8d69-ff15b68d73d9.png)
    
    Create a Pull request to make the changes in the original file.
    
    Note: The pull request will now send to the author of the repository and if accepted the changes will be made to the original repository.
    

# Week03 - IBM Tools for Data Science

## Watson Studio

## Other IBM Tools

- **Watson Knowledge Catalog**
    
    
- **IBM SPSS Modeler**
    - SPSS Modeler is a data mining and text analytics software application. It's used to build predictive models and conduct other analytics tasks. It has a visual interface that enables users to leverage statistical and data mining algorithms without programming.
    - Overfitting
        - Overfitting is defined as having significantly higher accuracy on the training data. Data used for training the model then on tests or unseen data.
- **Model Deployment**
    - Some workflow solutions
        
        ![Untitled](2%20Tools%20for%20Data%20Science%20d51c4d90a2cb44d2964211d2dc965f0c/Untitled%2044.png)
        
        - Some old open standards
            
            ![Untitled](2%20Tools%20for%20Data%20Science%20d51c4d90a2cb44d2964211d2dc965f0c/Untitled%2045.png)
            
            ![Untitled](2%20Tools%20for%20Data%20Science%20d51c4d90a2cb44d2964211d2dc965f0c/Untitled%2046.png)
            
        
        Since the deep learning approach is getting popular and popular, the open standards such as PMML and PFA did not react quilckly enough for the proliferation.
        
        In 2017, Micrsoft and Facebook created an open source - ONNX (Open Neura Network eXchange)
        
        ![Untitled](2%20Tools%20for%20Data%20Science%20d51c4d90a2cb44d2964211d2dc965f0c/Untitled%2047.png)
        
        - The tool from IBM - Watson Machine Learning
            
            ![Untitled](2%20Tools%20for%20Data%20Science%20d51c4d90a2cb44d2964211d2dc965f0c/Untitled%2048.png)
            
- **AutoAI in Watson Studio**
    
    Automatically create machine learning model
    
    ![Untitled](2%20Tools%20for%20Data%20Science%20d51c4d90a2cb44d2964211d2dc965f0c/Untitled%2049.png)
    
- **OpenScale(Watson Studio)**
    
    ![Untitled](2%20Tools%20for%20Data%20Science%20d51c4d90a2cb44d2964211d2dc965f0c/Untitled%2050.png)
    

# Week04 - Final Assignment: Create and Share Your Jupyter Notebook

## Create and Share Your Jupyter Notebook