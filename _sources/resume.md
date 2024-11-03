# Resume

<style>
  .skills-grid {
    width: 100%;
    border-collapse: collapse;
  }
  .skills-grid td {
    width: 50%;
    padding-left: 20px;
    vertical-align: top;
  }
  .skills-grid ul {
    list-style-type: disc;
    margin: 0;
    padding-left: 20px; /* Indent for bullet points */
  }
</style>

## <u>Summary</u>

With over 4 years of experience as a Business Intelligence Analyst and 6+ years in the technology sector, I specialize in developing precise technical requirements and delivering impactful data-driven insights. My strong foundation in retail banking and the stock market deepens my expertise in risk assessment and financial analysis, while my passion for automation drives me to continuously optimize processes. I am skilled in data analysis, visualization, automation, and technical documentation, and I’m equally enthusiastic about sharing knowledge—especially within data analytics. Known for my commitment to excellence and dedication to learning, I thrive in environments that encourage growth, innovation, and collaboration.

## Professional Experience

````{dropdown}  Business Intelligence Analyst, BlueShore Financial, 2021 - Current

::::{grid}

:::{grid-item}
:columns: 5
![BlueShore Logo](./img/bsf_logo-230-53.svg)  
:::
:::{grid-item}
:columns: 7
<a href="https://www.blueshorefinancial.com/" target="_blank">Visit BlueShore Financial</a>
:::
::::

Blueshore Financial is a Credit Union headquartered in North Vancouver, BC, with assets under management of $9+ billion. They offer a wide range of banking, wealth management, and insurance services tailored to meet the needs of individuals, businesses, and professionals. BlueShore emphasizes financial wellness and holistic planning, integrating innovative technology with high-touch client services to deliver a premium banking experience. 

::::{tab-set}

:::{tab-item} Job Overview
The Business Intelligence department is a small team of 3 (myself included) requiring us to work independantly (most of the time) - but also collaboratively with stakeholders to define and enact business requirements. 

I work with all areas of the business, including executive levels, Retail Branches (and their management), Business Process Solutions team, Finance, Treasury, Internal Banking Services and external partners too. This has given me exposure to all areas of the business.

On a typical business day, I will be working on a variety of projects, including any long term, multi-department projects, providing solutions to ad-hoc data requests from all areas of the Credit Union, attending meetings to assist in defining requirements, and providing training to staff on how to use tools.

I am given freedom to work on what I like as long as my deadlines are met and I love this as I can be creative and look to create new tools based on my 'side of the desk' ideas. An example of this is explained below (Mortgage Dashboard and Fraud Analysis).

I have worked remotely in this role since 2020.

:::
:::{tab-item} Responsibilities
- **Maintaining and creating dashboards on Power BI Server as well as adminstrating the server.** This includes determining the roles that can and cannot view various reports, and adding their permissions. Troubleshooting data refresh problems to ensure our users are being served the freshest and most accurate data. When creating dashboards, often there will be a series of meetings to define the problem, discuss the solution and refine the data points needed for the solution. Following is an iterative process to bring in the data from various databases / data sources, build the data models on Power BI, determine the best visuals (keeping the look and feel of the company theme), and then hosting on the DEV/QA and finally PROD servers. Lastly, there will be some kind of a presentation of the tool to others with a questions and answers part so that users can understand what the tool does and how to use it.
- **Attending Data Integrity Committee.** Every 2 weeks, 10-15 employees get together to discuss all things data so that we understand any developments, bugs or other issues around the data.
- **Providing ad-hoc data requests to various deparments.** Often someone will reach out wanting to know something specific about a certain subset of data that does not require a dashboard to be built, but does require some exploratory data analysis. Often outputting this to a spreadsheet will satisfy their needs. When discussing the needs, I always look to understand if this is a truely 1-off request, or if this is something they are likely to need in the future. For example, a 1-off request might be looking at a specific date range of data - whereas they may ask for a month end analysis but not realise that this would be helpful to see for the upcoming months too. Establishing this early allows me to create a better tool for them. A go-to solution might be for some dynamic SQL queries, embedded into a Power Query driven Excel spreadsheet - and perhaps some VBA if needed.
- **Learning the data sources and structures.** As with any data related role, you have to learn the data and that takes time. For my role, BlueShore financial has around 10-15 servers, each with 10+ databases - many of which are from external vendors and have their own rules about the way they work. For example, some are snapshot only with no history, others we received a full database each week and so there is an intricate time system to understand which segments you should be looking at. Most of the data is brought into a centralised data warehouse which has data cubes amd various views to interact with. Knowing what each cube is for (broken down into Customer, Account, Account Joints, Client, Collateral, Account Transaction) and  where the data from each cube comes from is vital to perform the job.
- **Reviewing, discussing and providing solutions for regulatory reporting.** Often we would receive requests from regulators to create reports based on our entire portfolio of clients. These reports often required multiple hundreds of datapoints for each client / loan and at any given time, there are around 5 or so regulatory reports I am responsible for creating, maintaining, updating, sending and discussing. As time has gone on, the reporting criteria and complexity has increased. In 2020, many of the regulatory reports could be run on a Power Query / SQL Server ETL combination. Now however, with the increasing amount of dataa sources needed for reports, and datapoints asked for significantly increasing, I have switched reporting to Python based using Jupyter Notebooks as this allows for easy, multi media user documentation and notes.
:::
:::{tab-item} Projects

```{dropdown} Anti-Money Laundering Data Aggregation Tool

Developed an anti-money laundering tool that aggregated and analyzed data from multiple banking systems to identify and prevent e-transfer money laundering activities. Leveraging Python and advanced regular expressions, the tool extracted and highlighted critical data patterns indicative of suspicious transactions.

The project involved integrating data from multiple banking sources into a centralized repository, allowing for streamlined analysis and insights. Through this tool, we identified telltale signs of money laundering in business and personal accounts. Key learnings included recognizing patterns such as business accounts receiving multiple transfers from various sources and personal accounts with low credit scores frequently engaging in high-volume transactions from multiple senders.

Upon deployment, the tool successfully flagged and provided evidence for several money-laundering schemes, leading to the immediate shutdown of operations. One notable case prevented a $10M+ money-laundering operation, directly contributing to regulatory compliance and safeguarding the institution’s integrity.

```
```{dropdown} Machine Learning - Credit Card Fraud Analysis

Started as a 'side of my desk' project where I was looking to apply my machine learning skills to a business problem. The particular problem was a specific subset of credit card fraud with a very imbalanced dataset. My first steps were to gather the data on these particular fraud cases - which in itself was not easy since I quickly found out that there was not a centralized repository for recording these fraud events. Instead, there was 2 departments, knowing some of what the other departments did but not all. Once I had reconcilled eachothers records, I went data mining in our client management system and found some stragglers. After exploring the data I developed some features started training, tuning and reviewing various algorithms to determine what would provide the best scoring metic. The model I settled on was a logistic regression classification algorithm which I chose to help with intepretability. I ultimately provided the data as an output table in deciles which the relevant department would review and reachout to clients to confirm transactions. The top 5% predicted about 90% of the actual fraudulent transactions and was used by the banking team.
```
```{dropdown} Power BI - Mortgage Dashboard

Another 'side of my desk' project without direction, I wanted to have a visualization of all things mortgages where you could explore everything in one spot. This was partly driven by the want to update our many, many Excel reports and condense them all into one location as a Power BI Report - getting rid of the older Excel reports. After some careful consideration of what various departments would find useful, I was able to create around 15 different tabs of different views along with various KPIs that were specific to each view. Some examples of these pages include, Mortgage View / Line of Credit View - a comprehensive view of our entire book of mortgages and lines of credits over time complete with branch breakdown tooltips, filters by various customer level and account level segmentations. Some KPIs developed showed $ increase over time, # increase over time, Account Utilization (for Lines of Credits) as well as total dollars over time. Another example of this tab was the Renewals and Fundings tab. This allowed users to see the renewals and fundings over time, again with the same customer and account level segmentation filters, as well as branch level breakdowns. I am proud to say that within the span of a couple of months, this went to being (by far) the most used dashboard, both on session count and time spent browsing in the credit union.
```
```{dropdown} VBA - Excel Tracking

Over the years, there has been a significant accumulation of Excel based reports building up in our centralised data reporting centre. The problem is that due to the way these reports were accessed, we had no idea who was using the reports (if anyone), and we were wanting to shift our reporting from Excel to Power BI based. I started researching how this could be done and came up with the following solution. Embedded VBA code which triggered on open of the spreadsheet that called a stored procedure I made which recorded the user name, the spreadsheet name, the location of the spreadsheet and some other important metadata. Once I got the go-ahead from IT Security (they had to whitelist the VBA code), I started implementing this on all our spreadsheets and added the tracking to my tracking dashboard which also monitored our SSRS and Power BI access. This has allowed us to see who is using the spreadsheets, and we had numerous benefits from this such as reducing the count of reports on our server, reaching out to power users of reports when developing new reports, understanding which reports are the key reports and getting a deeper understanding about how our reports are used by the organization.
```
```{dropdown} Regulatory Reporting

In late 2023, British Columbia Financial Services Authority provided guidelines on a new report which would be required by 2024 (end of year), that broke down our entire portfolio into retail and commercial loans (2 data extracts) - with about 200 datapoints for each loan. After reviewing and defining every data point, I created a shortlist of database developments needed for the mandatory fields that we were missing, help meetings with the relevant parties to initiate database development (mostly ETL processes from external data sources to our data warehouse). The report was prepared using a Jupyter Notebook as this is easy to export as an HTML file and provide regulators if they are asking about how we obtained the data, and using Python with Pandas and Numpy libraries. The report was well structured with only 2 variable to input in order to start the report, provided the relvant output files as well as outputting a data report for column by column analysis (library ydata-profiling). I also defined a number of assert statements which would flag if the criteria were not met, providing automated data checks along the way.
```
```{dropdown} Report Reporting - One Report to Rule them all!
Once we had a suite of Power BI, Excel and SSRS reports up and running, we didn't actually have any sightline into who was using these. I set about to build a dashboard which brought together Excel, SSRS, and Power BI Dashboards (seperated by Dev, QA and Prod) into one place. The tabs I created included Session counts by Source (Power BI, Excel, SSRS) - which was filterable by date, job titles, employees and reports. I also created some logic to determine how long reports were being used for based on what I defined as a session, and then rolled these up to report levels allowing us to see which reports were most used rather then simply most opened.
```
:::
:::{tab-item} Tools Used

%-----------Leave above


````{grid}
:gutter: 2

```{grid-item}
- SQL Server 
- Python
- SSAS Cubes
- Azure DevOps
```
```{grid-item}
- Jupyter Notebook
- M-Language
- SSRS Reports
- Skype
```
```{grid-item}
- Excel
- DAX
- VBA
- Outlook
```
````

%---------Leave Below
:::
::::


````{dropdown}  Senior Credit Analyst, BlueShore Financial, 2020 - 2021

::::{grid}

:::{grid-item}
:columns: 5
![BlueShore Financial Logo](./img/bsf_logo-230-53.svg)  
:::
:::{grid-item}
:columns: 7
<a href="https://www.blueshorefinancial.com/" target="_blank">Visit BlueShore Financial</a>
:::
::::

Blueshore Financial is a Credit Union headquartered in North Vancouver, BC, with assets under management of $9+ billion. They offer a wide range of banking, wealth management, and insurance services tailored to meet the needs of individuals, businesses, and professionals. BlueShore emphasizes financial wellness and holistic planning, integrating innovative technology with high-touch client services to deliver a premium banking experience. 

::::{tab-set}
:::{tab-item} Overview
This roles primary responsibility was the collection, analysis and reporting of the companies delinquent and higher risk lending. This required monthly reports to the organizations lending committee exectives as well as coaching of a small team of staff (3 others) on their branches which they looked after. I was also responsible for overseeing the payments of a $75m leading portfolio, including filing legal actions with our lawyers and attending small claims courts where neccessary.

I previously worked in the non-senior position for the same company back in 2014 and was proactively reached out to by my boss asking for me to come back. As described in my [Education](#education) section, at this point I was already committed to working in Business Intelligence - so this role was not exactly what I was after, however, I liked my boss and the company and so came back, letting my boss know I was interested in moving to the Business Intelligence department and asked that, if I committed a year to this role, would my boss support me moving onto the next role - which was agreed. I was also happy at the thought of applying some of my automation skills at the current processes within this role since I knew there would be plenty of opportunity.
:::
:::{tab-item} Responsibilities
- Automated a number of reported using a limited amount of Microsoft Office tools.
- Monitoring and reporting on a $75m portfolio of leases, including following up with clients and negotiation of payments where neccessary.
- Monthly presentations to the lending committee on KPI indicators for lending and leasing portfolios as well as providing any relevant updates for higher risk loans.
- Coaching a smaller team for their weekly duties.
- Filing legal action and travelling to small claims court where neccessary.
:::
:::{tab-item} Projects
**Excel Based Reporting - Updates**

I found the reporting to be quite cumbersome since it was dominated by Excel spreadsheets and due to security requirements, I wasn't able to download any Python related tools, however, I realised that I could simply use the existing embedded VBA within Excel to automate the majority of the work. I therefore spent the next few months learning and updating the reporting so that the bi-monthly and monthly reports could simply be run by VBA based macros which saved a considerable amount of time. For example, the monthly leasing tracking which previously took 1 hour of manual clicking each month was now resolved in about 5 minutes with 95% of the work being completed by clicking the run-macro button.

**Client Credit Score Analysis**

As a drive to reduce our risk, we drilled into our client credit reports and determined metrics to assess a clients risk profile. Once we looked at the overall numbers we were dealing with, we proactively contacted clients and managed to de-risk the high risk lending by greater then $4m over a short period. 
:::

:::{tab-item} Tools Used

%-----------Leave above


````{grid}
:gutter: 2

```{grid-item}
- Excel
- VBA
```
```{grid-item}
- SSAS Cubes
- SSRS Reports
```
```{grid-item}
- Skype
- Outlook
```
````

````{dropdown}  Business Analyst, Quotemedia, 2019-2020

::::{grid}

:::{grid-item}
:columns: 5
![Quotemedia Logo](./img/quotemedia_logo-207x115.png)  
:::
:::{grid-item}
:columns: 7
<a href="https://www.quotemedia.com/" target="_blank">Visit Quotemedia</a>


:::
::::

QuoteMedia operates mainly as a Software as a Service (SaaS) company, and is a leading data provider, web software developer, data aggregator, and syndicator of unique, private labeled financial content and streaming financial data solutions. QuoteMedia provides to online brokerages, clearing firms, banks, financial service companies, media companies, Internet portals, and public corporations.  

::::{tab-set}
:::{tab-item} Overview
Working as the Business Analyst for all parts of the company which were broken down into segments, including loading of data, XML API data, Quotestream (SaaS product), microservices and streaming. This required knowledge of all areas of the business including the underlying details on the stock market such as options chains, clearing houses, SEC, SEDAR and more. I was the go between for developers and the stakeholders, both internal and external and held morning scrums, planned releases, patches and produced patch notes which was distributed to clients. 
:::
:::{tab-item} Responsibilities
- Delivering end to end implementation of financial market SaaS products including transactional portfolio, elastic News Search with Kibana, stock screener, market maker modules, historic and real time stock market graphs and analytics.
- Led 5 Scrum teams while owning the plan, design, development, UI prototype, and deployment of financial contents.
- Responsible for managing product roadmap, vision, end to end release planning, and drive improvements for QuoteStream.
- Planned and executed change management strategies for Market data fundamental and logical calculation updates, Vendor licensing switch, and Legacy system migration impacting more than 15K users.
- Responsible for User Acceptance Testing (UAT) for XML/JSON APIs, Web content solutions and Market data reports.
- Developing business requirements from the stakeholders with the developers and planning them into workflows.
- Documentation of releases/patch notes.
- Holding weekly team meetings to plan sprints and determine / resolve any roadblocks.
- Communicating between all areas of the business so that all stakeholders are aware of estimated delivery dates of various features.
- Grooming the bug tickets and miscellaneous ticket queues and fitting them into workflows.
:::
:::{tab-item} Projects
**Changed Data Sources**

In an effort to reduce costs, a deal was made with an external company that would provide similar data to the financial data supplier, Morningstar. Part of my role was to provide an overview of the data needed and review the data they produced, comparing it to our current data. This was done over their API using an Oracle database to generate and review differences in data.
This project took around 9 months to fully complete and there were a variety of issues, not only with data quality, but also API performance which had to be resolved.

**Planning of a Major Code Update**

The loading scripts used for the company were quite complex and had ~150,000 lines of code. With the loading team turnover being quite high, and the large amount of code, there wasn't anyone that knew exactly what all the code did. In an effort to simplify the process, I worked with the loading team to breakdown the script into a series of modules, providing data quality and analysis along the way.
:::

:::{tab-item} Tools Used

%-----------Leave above


````{grid}
:gutter: 2

```{grid-item}
- Excel
- Oracle
```
```{grid-item}
- Postman API
- Jira
```
```{grid-item}
- Slack
- Confluence
```
````



````{dropdown}  Technical Support (Level 1 & 2) , Quotemedia, 2017-2019

::::{grid}

:::{grid-item}
:columns: 5
![Quotemedia Logo](./img/quotemedia_logo-207x115.png)  
:::
:::{grid-item}
:columns: 7
<a href="https://www.quotemedia.com/" target="_blank">Visit Quotemedia</a>


:::
::::

QuoteMedia operates mainly as a Software as a Service (SaaS) company, and is a leading data provider, web software developer, data aggregator, and syndicator of unique, private labeled financial content and streaming financial data solutions. QuoteMedia provides to online brokerages, clearing firms, banks, financial service companies, media companies, Internet portals, and public corporations.  

::::{tab-set}
:::{tab-item} Overview
Required working knowledge of all areas of the business, which included loading of data, XML API data, Quotestream (SaaS product), microservices and streaming, in order to understand issues from the ticketing platform Zendesk, and then research the issues using the companies internal knowledge database which included Jira and Conflueuence. Keeping clients up to date or providing remote desktop training was routinely required. In these roles, level 1 took the tickets and solved the easier ones, level 2 actually looked into the database, fixed data intergrity/quality issues and referred items for development where needed.
:::
:::{tab-item} Responsibilities
- Production support for Java and web based products
- Monitor and maintain the quality and accuracy of financial stock market data received from a variety of sources
- Proactively analyze company products, providing solutions to improve their quality
- Review data, applications and configurations to resolve incidents and prevent re-occurrences
- Work with the development and quality assurance teams to plan and test software deployments
- Improve company documentation on task procedures and enhancements
- Liaise with data vendors (TMX, Nasdaq, Morningstar) on operational issues as required
- Keeping on top of tickets from clients that either needed in depth analysis or a brief response to inform the client of how to use product properly.
- Remotely connecting to clients to show them how or witness software issues.
- Using stored procedures to fix indices that would either break or need monthly balancing.
- Keeping track of items being worked on so that clients expectations are in line with workflows.
- Understanding the various payment structures of the SaaS platform in order to coach the users on what data entitlements they needed.
:::
:::{tab-item} Projects
**Indices Administration**

The company decided to create custom indices for clients that requested them which would then be displayed on their propriatory website widgets, QMOD. The indices would have to be regularly balanced and often the underlying stock tickers that made up the indices would change which would require database work to resolve the problem.

**Data Integrity Issues**

We often would get questions from more advanced users about Options chains or Volume Weighted Average calculations that would require research from the developers and / or knowledge base. This would then be documented for future use when the client asked about something similar.
:::

:::{tab-item} Tools Used

%-----------Leave above


````{grid}
:gutter: 2

```{grid-item}
- Excel
- Oracle
- Linux
```
```{grid-item}
- Zendesk
- Jira
```
```{grid-item}
- Slack
- Confluence
```
````
````{dropdown}  Financial Advisor, Drewberry Insurance, 2016-2017

::::{grid}

:::{grid-item}
:columns: 5
![Drewberry Insurance Logo](./img/drewberry_logo-200x120.png)  
:::
:::{grid-item}
:columns: 7
<a href="https://www.drewberryinsurance.co.uk/" target="_blank">Visit the Drewberry Insurance</a>
:::
::::

Drewberry Insurance are a team of UK financial planners with offices in London and Brighton.

They provide regulated financial advice services to individuals and businesses throughout the UK on a wide range of topics from protecting ones personal finances or managing their wealth to setting up Employee Benefits for large UK companies.
::::{tab-set}
:::{tab-item} Overview
Providing regulated financial advice for personal and business clients, specialising in Life, Critical Illness & Income Protection for private clients, including self-employed and high net worth individuals. As well as Business Protection Insurance (Key Person, Shareholder Protection, Directors Insurance) for a diverse range of clients from start-up's, SMEs, to larger corporations.
:::
:::{tab-item} Responsibilities
- Advising clients and sending recommendations for a range of protection products
- Generating referrals from clients
- Negoaiating terms with insurance vendors on the clients behalf
:::

````

