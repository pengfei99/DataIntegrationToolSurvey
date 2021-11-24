# Data Integration Tool Survey

## 1.What is data integration?

**Data integration** is the process of combining data from different sources into a single, unified view. Integration 
begins with the ingestion process, and includes **steps such as cleansing, ETL mapping, and transformation**. Data 
integration ultimately enables analytics tools to produce effective, actionable business intelligence.

### A typical data integration process
The client sends a request to the master server for data. The master server then intakes the needed data from 
internal and external sources. The data is extracted from the sources, then consolidated into a single, cohesive 
data set. This is served back to the client for use.


## 2.ETL, ELT and data integration
ETL(Extract, Transform, Load) and ELT (Extract, Load, Transform) are both processes within data integration where
data is taken from the source systems(internal or external) and delivered into the destination.

With the rise of data lake, the ELT pattern becomes more and more popular. So the data transformation is no longer a 
must-have. A data integration tool can be as simple as a tool which copies and past data.

## 3. Challenges to data integration
Taking several data sources and turning them into a unified data structure is a technical challenge. Below are some 
common challenges that data integration tool will face:
- understand the context: Anyone who implements data integration process must understand 
   - what types of data need to be collected and analyzed, 
   - where that data comes from, 
   - which system will use the integrated data
   - what types of analysis will be conducted
   - how frequently data and reports will need to be updated.
- Data from legacy systems: Integrate data stored in legacy systems
- New data sources:  New systems today are generating different types of data (such as unstructured and binary data ) 
  from all sorts of sources such as IoT devices(e.g. sensors), and cloud. The integration system needs to quickly adapt
  the new sources and fulfil the requirements such as:
    - Volume
    - Velocity
    - the new format of data.
- Continues maintenance: The task is not done even after your integration system is up and running. We need to keep it
  up to date with the latest demands from the organization and regulatory agencies (GDPR) with respect of the best practices.

## 4. Different types of data integration
- Manual data integration: Use pseudo scripts that interface directly with sources and load data to destination. This is 
  highly inefficient and inconsistent.
- Middleware data integration: Use middleware applications that acts as a mediator, to normalize data and bring it
  into the destination master data pool. Legacy applications often don’t play well with others. Middleware comes into 
  play when a data integration system is unable to access data from one of these applications on its own.
- Application-based integration: Use software applications to locate, retrieve, and integrate data. During 
  integration, the software must make data from different systems compatible with one another, so they can be 
  transmitted from one source to another.
- Uniform access integration: Use a front-end that makes data appear consistent when accessed from different sources. 
  But the data is left within the original source. When a user requires a data, the engine will do the ETL en live by
  retrieving data from various data 

## 4. General feature of data integration tools

## 5. Metrics to mesure data integration tools

- Connectors: The more pre-built connectors that your tool has, the more time your team will save to connect to a data source
- Scalability: Ensure that the tool can easily scale up and down (scale horizontally is preferred)as per your data needs
- Portability: The ETL script and the tool environment should be able to run anywhere (e.g OS or infra)
- Security and compliance: ensure the tool address security and compliance issues
- Real-Time: Not all companies need to do real-time analysis. As a result, not all Data Integration tools support this. 
  Many bring data to the destination in batches – creating a lag of anywhere between a few hours to days.
- Advance data transformations: To do advance data transformation, it needs to be able to read various data format and
  modify values in it. For example, one csv has timestamp format <mm-dd-yy>, one postgresql table has <dd-mm-yy>. After 
  transformation, we want the timestamp to be <yy-mm-dd>
- Ease to use: Data integration tools should be easy to learn and easy to use with a GUI interface to make visualizing your data pipelines simpler.
- Cloud Native: The data integration tool should work natively in a single cloud, multi-cloud, or hybrid cloud environment.
- Price: Opensource vs proprietary. The price of opensource solution is mainly in HR, because you will not get fast bug
  fixing. For the proprietary tool, it must have a transparent price model.


## 6. Existing tool 

### 6.1 Proprietary tools:

|Tools|Type	|Transparent Pricing|No-Code Interface|	Purchase process|G2 customer satisfaction|
|-----|-----|------------------|-----------------|-------------|----------------|
|Hevo Data |Commercial|	Yes	|Yes|Self-Service|4.8/5|
|Dell Boomi	| Commercial|Yes|Yes|Self-Service	|4.2/5|
|Informatica| Commercial	|No	|Yes	|Contact Sales	|4.4/5|
|Talend	|Open-Source	|No	|Yes	|Contact Sales	|4.0/5|
|Pentaho	|Open-Source|	No	|Yes	|Contact Sales	|4.3/5|
|SnapLogic|	Commercial	|Yes	|Yes	|Self-Service	|4.2/5|
|Jitterbit	|Commercial	|No	|Yes	|Contact Sales	|4.7/5|
|Zigiwave	|Commercial	|Yes|	Yes	|Contact Sales	|4.8/5|
|IRI Voracity	|Commercial	|No	|Yes	|Contact Sales	|None|
|Oracle	|Commercial	|Yes	|Yes	|Self-Service	|4.0/5|
|Celigo	|Commercial	|Yes	|Yes	|Self-Service	|4.6/5|
|MuleSoft	|Commercial	|No	|No	|Contact Sales	|4.5/5|

### 6.2 Open source tools

- Flume
- Meltano
- NiFi
- 