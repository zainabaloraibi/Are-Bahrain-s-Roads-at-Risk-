# Are Bahrains Roads at Risk?
Data-driven analysis of the 2018 Hawkeye Road survey conducted in Bahrain. The goal is to identify pavement defects across road segments and support the development of an efficient and informed road maintenance plan based on actual condition data.

## 1.	Introduction
Road condition assessment is a key component of pavement management, particularly in countries with harsh climates and growing urban infrastructure like Bahrain. In 2018, a comprehensive pavement survey was conducted using the Hawkeye system, targeting major road segments across Bahrain. The purpose of this data collection was to evaluate surface and structural conditions and support future maintenance and rehabilitation planning.
The dataset includes a wide range of pavement distresses, each reflecting a specific type of degradation that affects road performance and safety. These include:
•	IRI (International Roughness Index): Measures the smoothness of the road. A higher IRI indicates a rougher, less comfortable driving surface.
•	Cracks: Visible breaks or fractures in the pavement surface, often caused by aging, thermal expansion, or traffic loads.
•	Potholes: Bowl-shaped depressions formed due to surface failure, often worsened by water infiltration and repeated loading.
•	Rutting: Longitudinal surface depressions in wheel paths caused by repeated traffic, especially from heavy vehicles.
•	Texture: Refers to the micro-roughness of the pavement, which affects tire grip and water drainage.
•	Raveling: The disintegration of the surface layer as aggregate particles come loose, usually due to binder aging or poor compaction.
Each road segment in the dataset is georeferenced and assessed using severity-based ratings for these distresses. This allows for a comprehensive understanding of pavement health across Bahrain’s main roads and supports data-driven decision-making in infrastructure maintenance.

## 2.	Problem Statement
The Hawkeye survey is a road assessment system that uses cameras and sensors to inspect pavement conditions. It was conducted in Bahrain during the last two weeks of December 2018, covering most major roads.

## 3.	Objectives
•	Analyze pavement condition data collected from the Hawkeye survey across Bahrain.
•	Calculate the percentage distribution of pavement distresses.
•	Calculate the percentage distribution of pavement distresses by severity level
•	Identify the most common types of pavement distresses in Bahrain 
•	 Determine which lanes show higher deterioration levels based on rutting.
•	 Assess which zones are more deteriorated based on cracking severity.
•	  Evaluate the severity and frequency of potholes across the network.
•	 Identify the most frequently required pavement treatments based on distress severity.
•	 Rank the top three roads with the highest levels of poor condition.
•	 Explore the relationship between surface texture and International Roughness Index (IRI).
•	 Locate critical areas that require reconstruction due to severe deterioration.

## 4.	Target Audience
•	Ministry
•	Consultant firms
•	Contractor companies 

## 5.	Dataset(s)
The dataset is a detailed pavement condition survey collected using the Hawkeye system, covering road segments across Bahrain. It contains geospatial coordinates, surface condition measurements, and structural distress indicators. The data primarily focuses on main roads.

## 6.	Data Handling
Unnecessary Columns Removed:
The following non-essential columns were dropped:
'ROAD NAME', 'Unnamed: 1', 'ANALY-SIS', 'SECTION', 'Unnamed: 8', 'SURVEY DATE', 'EVENTS', 'DIRECTION', 'LANE NO.', and 'SUB CHAINAGE'.
Geolocation Validation:
Records outside Bahrain’s geographic boundaries were identified and removed. A total of 94 records (less than 10% of the dataset) were excluded.
Column Renaming:
Columns with unclear or unnamed headers were renamed to meaningful labels for clarity and consistency.
Handling Missing Values:
Null values were identified and handled accordingly.
For the Potholes Severity column, missing values were filled based on their corresponding Potholes Rating.
Remaining null values, accounting for less than 10% of the data, were dropped to maintain data integrity.
Replacing Placeholder Values:
Placeholder values marked as 'X' in multiple columns were reviewed.
After verifying the corresponding rating columns, 'X' was replaced with 0, as the rating confirmed the absence of the defect.
Data Type Conversion:
Columns were converted to appropriate data types (e.g., numeric) to allow accurate computations and analysis.



## 7.	Analysis and Findings

•	There is a direct relationship between IRI and cracks; higher cracking leads to higher IRI values.
•	Zone 2 is identified as the worst-performing zone, with the highest number of cracks.
•	Potholes are classified as low severity across the network.
•	The Capital Governorate has the highest number of road distresses, as it contains many of the oldest roads in the country.
•	Routine maintenance, including 50 mm overlay, is the most suitable treatment in many areas.
•	Reconstruction should be prioritized in the most deteriorated points, which are located at intersections due to frequent braking and turning.
•	The top 3 most deteriorated roads are:
1.	National Charter Road
2.	Al Nakheel Highway
3.	Shaikh Jaber Al-Sabah Highway
   
## 8.	Recommendations
1-	Focus on Zone 2, the most deteriorated Zone. Prioritize crack repair, as it raises IRI and lowers ride quality.
2-	Prioritize maintenance in the Capital Governorate due to its highest pavement distress There.
3-	Use interlocking pavers at intersections for easier maintenance, and high-strength concrete in high-traffic areas for greater durability.
  	
## 9.	Limitations and Assumptions
Lack of Traffic Data:
Traffic volume information is not available, making it difficult to analyze the relationship between distress levels and traffic loading.
Missing Units in Some Columns:
Several data columns lack specified units. Reasonable assumptions were made where possible, which may introduce minor uncertainties.
Absence of Historical Data:
The dataset only represents a single point in time. Without historical records, it is not possible to assess how road conditions in Bahrain have changed over time.
Limited to Main Roads Only:
The dataset covers only main roads. Data for secondary or internal roads is missing, limiting the comprehensiveness of the analysis.

