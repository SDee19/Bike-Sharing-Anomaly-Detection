![360_F_1932418825_rXTmTxlTw1OSmnNKuZvhOQWVnilu96G5](https://github.com/user-attachments/assets/ed110eb8-ed9a-4152-a6f9-5df98a1c0500)


# Bike-Sharing-Anomaly-Detection
This project investigates the potential of urban "𝗕𝗶𝗸𝗲-𝗦𝗵𝗮𝗿𝗶𝗻𝗴" data as a real-time, non-intrusive sensor network for broader urban intelligence and public safety. Moving beyond conventional applications like demand forecasting, this study employs Exploratory Data Analysis (EDA) and Advanced Machine Learning to detect localized, statistically significant anomalies in hourly bike rental patterns. The initial EDA establishes baseline activity across various temporal (hourly, seasonal) and environmental 
(weather) contexts. Building on this foundation, an XGBoost model (the optimum one) is implemented to learn "𝗻𝗼𝗿𝗺𝗮𝗹" usage from historical data (2011) and flag significant deviations in subsequent data (2012). The results demonstrate the model's ability to identify unusual surges or drops in activity that correlate with phenomena such as public events, infrastructure disruptions, or potential emergencies. The insights are materialized in a data product, CityPulse, a web-based dashboard designed for Urban 
Planners, Public Safety Officials, and City Management. "𝗖𝗶𝘁𝘆𝗣𝘂𝗹𝘀𝗲" transforms high-resolution mobility data into a proactive, early-warning mechanism, offering enhanced situational awareness and enabling data-driven decision-making for managing urban disruptions and improving public safety.


# Description of the Question 

"𝗖𝗮𝗻 𝗺𝗮𝗰𝗵𝗶𝗻𝗲 𝗹𝗲𝗮𝗿𝗻𝗶𝗻𝗴 𝗺𝗼𝗱𝗲𝗹𝘀 𝗲𝗳𝗳𝗲𝗰𝘁𝗶𝘃𝗲𝗹𝘆 𝗱𝗲𝘁𝗲𝗰𝘁 𝗮𝗻𝗼𝗺𝗮𝗹𝗼𝘂𝘀 𝗽𝗮𝘁𝘁𝗲𝗿𝗻𝘀 𝗶𝗻 𝗵𝗼𝘂𝗿𝗹𝘆 𝗯𝗶𝗸𝗲-𝘀𝗵𝗮𝗿𝗶𝗻𝗴 𝗿𝗲𝗻𝘁𝗮𝗹 𝗱𝗮𝘁𝗮, 𝗰𝗼𝗻𝘀𝗶𝗱𝗲𝗿𝗶𝗻𝗴 𝘀𝗲𝗮𝘀𝗼𝗻𝗮𝗹, 𝘄𝗲𝗮𝘁𝗵𝗲𝗿, 𝗮𝗻𝗱 𝘁𝗲𝗺𝗽𝗼𝗿𝗮𝗹 𝗳𝗮𝗰𝘁𝗼𝗿𝘀, 𝘁𝗼 𝘀𝗲𝗿𝘃𝗲 𝗮𝘀 𝗮𝗻 𝗲𝗮𝗿𝗹𝘆 𝗶𝗻𝗱𝗶𝗰𝗮𝘁𝗼𝗿 𝗳𝗼𝗿 𝗹𝗼𝗰𝗮𝗹𝗶𝘇𝗲𝗱 𝘂𝗿𝗯𝗮𝗻 𝗮𝗰𝘁𝗶𝘃𝗶𝘁𝘆 𝗱𝗶𝘀𝗿𝘂𝗽𝘁𝗶𝗼𝗻𝘀 𝗼𝗿 𝗽𝗼𝘁𝗲𝗻𝘁𝗶𝗮𝗹 𝗽𝘂𝗯𝗹𝗶𝗰 𝘀𝗮𝗳𝗲𝘁𝘆 𝗰𝗼𝗻𝗰𝗲𝗿𝗻𝘀?" 

The fundamental problem for city stakeholders—including Public Safety Officials, Urban Planners, and City Management—is the lack of a real-time, non-intrusive early-warning system to monitor localized urban activity and potential public safety threats. Traditional urban monitoring relies on siloed data sources, but bike-sharing systems generate a rich, dynamic dataset that reflects the granular patterns of human movement across the city. The challenge addressed by this project is to move beyond the 
conventional use of this mobility data (such as demand prediction or system optimization) and transform it into a powerful urban sensor network. 

The core problem is the necessity to accurately identify unusual deviations in hourly bike rental patterns that could signify unexpected events, urban disruptions, or precursors to public safety incidents. The existing gap is the industry's inability to leverage complex temporal, seasonal, and weather factors to establish a robust baseline of "normal" urban flow, thereby preventing the proactive detection of anomalies. The objective of this project is to develop and implement machine learning models to effectively detect these anomalous patterns, providing an early indicator for localized activity disruptions and enabling a shift from reactive analysis to proactive urban management and enhanced situational awareness.

# Description of the Dataset

The Bike-Sharing dataset contains detailed historical data on the Capital Bikeshare system in Washington D.C., recorded over two years (2011-2012). It captures the hourly (17,379) and daily (731) count of rental bikes, enriched with corresponding temporal, seasonal, and weather information. 

<img width="1185" height="606" alt="Screenshot 2026-03-29 081948" src="https://github.com/user-attachments/assets/27c93808-fbeb-4057-8124-8634470fc806" />

𝗟𝗶𝗻𝗸 𝗳𝗼𝗿 𝘁𝗵𝗲 𝗱𝗮𝘁𝗮𝘀𝗲𝘁: https://archive.ics.uci.edu/dataset/275/bike+sharing+dataset

# Conclusions and Discussion

The comprehensive analysis of the Bike-Sharing dataset, encompassing both Exploratory Data Analysis (EDA) and a supervised machine learning approach for anomaly detection, yielded significant insights into urban mobility patterns and the challenges of repurposing transportation data for public safety applications (CityPulse).


𝗜𝗻𝘀𝗶𝗴𝗵𝘁𝘀 𝗳𝗿𝗼𝗺 𝗘𝘅𝗽𝗹𝗼𝗿𝗮𝘁𝗼𝗿𝘆 𝗗𝗮𝘁𝗮 𝗔𝗻𝗮𝗹𝘆𝘀𝗶𝘀 (𝗘𝗗𝗔)

The EDA phase established that bike usage, measured by the cnt (total count of bikes rented), is highly deterministic, showing clear, predictable patterns governed by temporal and environmental factors. Key findings include: 

1. 𝗗𝗼𝗺𝗶𝗻𝗮𝗻𝘁 𝗧𝗶𝗺𝗲 𝗦𝗲𝗿𝗶𝗲𝘀 𝗘𝗳𝗳𝗲𝗰𝘁𝘀: Bike rentals exhibit strong periodicity. Daily patterns show characteristic peaks during morning and evening rush hours, while seasonal trends demonstrate a clear hierarchy: "Summer" and "Fall" are the peak seasons, with "Winter" having the lowest usage. 

2. 𝗘𝗻𝘃𝗶𝗿𝗼𝗻𝗺𝗲𝗻𝘁𝗮𝗹 𝗜𝗻𝗳𝗹𝘂𝗲𝗻𝗰𝗲: Weather is a critical driver. The "temp" and "atemp" variables show a high positive correlation with "cnt", confirming that warmer, ideal weather conditions lead to higher demand. Conversely, adverse conditions ("weathersit" equals to 3 or 4) drastically suppress usage. 

3. 𝗕𝗶𝗳𝘂𝗿𝗰𝗮𝘁𝗲𝗱 𝗕𝗲𝗵𝗮𝘃𝗶𝗼𝗿: Clustering analysis (K-Means) on the features effectively segmented the data into two primary clusters: "Low Demand" (dominated by off-peak hours and severe weather) and "High Demand" (representing peak seasons, working days, and rush hours). This validated the concept that a clear "normal" operating envelope exists, which became the foundation for defining anomalies. However, analysis across four statistical decision approaches (30 indices, the Elbow Method, Average Silhouette Width, and Gap-Statistics Method) indicated that these clusters were not statistically sound (lacked a clear, distinct boundary).


𝗔𝗱𝘃𝗮𝗻𝗰𝗲𝗱 𝗔𝗻𝗮𝗹𝘆𝘀𝗶𝘀: 𝗧𝗿𝗮𝗻𝘀𝗶𝘁𝗶𝗼𝗻 𝘁𝗼 𝗔𝗻𝗼𝗺𝗮𝗹𝘆 𝗗𝗲𝘁𝗲𝗰𝘁𝗶𝗼𝗻

To address the core problem of lacking an anomaly-flagged column, the analysis transitioned to a supervised learning framework. By utilizing the two-cluster split or a similar rule-based deviation from the expected mean, a binary target variable was engineered, converting the forecasting task into an anomaly classification problem. 

The optimized "𝗫𝗚𝗕𝗼𝗼𝘀𝘁 𝗖𝗹𝗮𝘀𝘀𝗶𝗳𝗶𝗲𝗿" emerged as the strongest predictive model, achieving the highest "𝗙𝟭-𝘀𝗰𝗼𝗿𝗲" (the critical metric for class imbalance and public safety applications, where both false negatives and false positives are costly). Feature Importance analysis confirmed that temporal features (hr, mnth, workingday) remained the most influential predictors, followed by the temperature variables (temp, atemp). This reinforced the EDA findings, demonstrating that the model was correctly learning the established "normal" temporal and environmental baseline.


𝗠𝗼𝗱𝗲𝗹 𝗣𝗲𝗿𝗳𝗼𝗿𝗺𝗮𝗻𝗰𝗲 𝗮𝗻𝗱 𝗦𝘆𝘀𝘁𝗲𝗺 𝗟𝗶𝗺𝗶𝘁𝗮𝘁𝗶𝗼𝗻𝘀

Despite the successful feature engineering and model optimization, two major constraints emerged: 

1. 𝗣𝗲𝗿𝘀𝗶𝘀𝘁𝗲𝗻𝘁 𝗢𝘃𝗲𝗿𝗳𝗶𝘁𝘁𝗶𝗻𝗴: Even with extensive hyperparameter tuning (as detailed in the tuning grid), the optimized model could not fully mitigate the gap between training and validation performance. This high variance indicates the model is overly specialized to the "2011" training data and may fail to generalize reliably to unpredictable urban events, posing a risk to the "CityPulse" system's fidelity in a live environment.

2. 𝗚𝗲𝗻𝗲𝗿𝗮𝗹𝗶𝘇𝗮𝘁𝗶𝗼𝗻 𝗕𝗮𝗿𝗿𝗶𝗲𝗿: The product is inherently limited by its reliance on historical, domain-specific data from "Washington, D.C." The highly localized influence of weather and temperature means the model’s performance is geographically constrained. Without significant retraining and localized data, "CityPulse" lacks the generalization required for implementation in other regional or international domains.


In conclusion, the project successfully developed and validated a predictive model that serves as the basis for the production of tool "𝗖𝗶𝘁𝘆𝗣𝘂𝗹𝘀𝗲" data, we have provided a tangible solution that allows urban management and public safety officials to move from a reactive stance to a proactive stance in monitoring urban activity, ultimately contributing to a safer and more resilient future for the city. data. By transforming complex historical bike share data into a simple, interpretable, and highly accurate predictive tool, we have provided a tangible solution that allows urban management and public safety officials to move from a reactive stance to a proactive stance in monitoring urban activity, ultimately contributing to a safer and more resilient future for the city.

# CityPulse - 𝑼𝒏𝒄𝒐𝒗𝒆𝒓 𝒕𝒉𝒆 𝒔𝒕𝒐𝒓𝒚 𝒃𝒆𝒉𝒊𝒏𝒅 𝒆𝒗𝒆𝒓𝒚 𝒓𝒊𝒅𝒆. 𝑻𝒓𝒂𝒄𝒌, 𝒑𝒓𝒆𝒅𝒊𝒄𝒕, 𝒂𝒏𝒅 𝒆𝒙𝒑𝒍𝒐𝒓𝒆 𝒚𝒐𝒖𝒓 𝒄𝒊𝒕𝒚'𝒔 𝒄𝒚𝒄𝒍𝒊𝒏𝒈...

1. 𝗛𝗼𝗺𝗲 𝗣𝗮𝗴𝗲

   ![WhatsApp Image 2026-03-29 at 10 51 47](https://github.com/user-attachments/assets/95aee3fd-c9ed-4941-bb52-0fa7d4f6c530)

2. 𝗜𝗻𝘁𝗲𝗿𝗮𝗰𝘁𝗶𝘃𝗲 𝗗𝗮𝘀𝗵𝗯𝗼𝗮𝗿𝗱

   ![WhatsApp Image 2026-03-29 at 10 51 48](https://github.com/user-attachments/assets/7b704043-a2da-4259-b21e-1c71c687d214)

3. 𝗣𝗿𝗲𝗱𝗶𝗰𝘁𝗶𝗼𝗻 𝗘𝗻𝘃𝗶𝗿𝗼𝗻𝗺𝗲𝗻𝘁

   ![WhatsApp Image 2026-03-29 at 10 51 48 (1)](https://github.com/user-attachments/assets/270c9e80-e0cd-4d9f-b922-7c151a9dc85c)

4. 𝗖𝗼𝗻𝘁𝗮𝗰𝘁 𝗨𝘀 𝗣𝗮𝗴𝗲

   ![WhatsApp Image 2026-03-29 at 10 51 49](https://github.com/user-attachments/assets/f3bd9965-7ba1-4f24-8d20-eef3a252b786)





