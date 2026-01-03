# Datasheet for the "Spirited Girls" Subculture Dataset

Following the framework proposed by Gebru et al. (2021), this datasheet provides a comprehensive overview of the dataset used in the study: "Decoding 'Spirited Girls': An Explainable Socio-Spatial Analysis of Platformed Subcultural Discourse in China."

## 1. MotivationPurpose

This dataset was created to analyze the thematic evolution and socio-economic drivers of the "Spirited Girls" (精神小妹) subculture on short-video platforms.Creators: The authors of the associated research paper.Funding: This research did not receive specific commercial funding; it was conducted for academic purposes.

## 2. CompositionTotal Records

333,327 effective comments (derived from a raw set of 746,724).Data Fields:Textual Content: Normalized user comments (Emoji-to-text conversion applied).Provincial IP Geolocation: The mandatory location tag disclosed by the platform.Like Count: Number of user "likes" for each comment.Timestamp: The exact time of posting.Temporal Coverage: September 7, 2022, to May 20, 2025.Representativeness: The data covers 34 provincial-level administrative regions in China, with significant concentrations in Guangdong, Henan, Shandong, and Jiangsu.

## 3. Collection ProcessMethod

Data was collected via a custom browser extension designed to extract fully rendered content from Douyin's web interface.Sampling Strategy: We utilized Douyin's fuzzy search for the keyword "Spirited Girls" and manually screened 191 high-engagement videos (>1,000 comments each) for thematic relevance.Timeframe: The collection was completed in May 2025.

## 4. Preprocessing, Cleaning, and LabelingCleaning

Removed non-semantic characters and control symbols.Filtered comments shorter than 6 Chinese characters to ensure discursive quality. Implemented Emoji-to-text conversion by stripping brackets from the platform's native [semantic_description] format.Anonymization: All Personally Identifiable Information (PII), including usernames, user IDs, and "@mentions," was stripped to protect privacy. Labeling: Thematic classification was performed using DeepSeek R1 via few-shot learning. Validation: A gold-standard set ($N=1,000$) was created through dual-independent manual labeling with a third-party tie-breaker.Accuracy: 90.80%; Inter-rater Reliability (IRR): 97.30%.

## 5. UsesIntended Use

Academic research into subcultural dynamics, platform governance, and computational social science.Restrictions: This dataset should not be used for regional profiling, stigmatization of specific educational cohorts, or the re-identification of individual users.

## 6. DistributionFormat

The core analytical code and a 10% anonymized sample are available via an anonymous GitHub repository.License: MIT License for the code.FAIR Principles: We adhere to the FAIR principles (Findable, Accessible, Interoperable, Reusable) by providing persistent URLs and standardized documentation.

## 7. MaintenanceSupport

The authors will maintain the repository for at least three years following publication.Updates: No major updates to the 2022-2025 dataset are planned, though the classification code may be updated for future compatibility.
