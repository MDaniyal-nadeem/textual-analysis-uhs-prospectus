# Textual Analysis of UHS 2025-26 Prospectus

## Project Overview

A comprehensive natural language processing and statistical analysis of the University of Health Sciences (UHS) 2025-26 prospectus document. This project applies text mining, frequency analysis, and probability assessment to extract meaningful insights from institutional communication materials.

## Objective

To apply statistical and computational text analysis methods to the university prospectus with the following goals:

1. Identify dominant themes and branding keywords through word frequency analysis
2. Assess document readability and linguistic complexity using descriptive statistics
3. Evaluate balanced messaging by analyzing keyword distribution across pages
4. Provide actionable insights for improving institutional communication and branding

## Scope

The analysis focuses exclusively on textual content from the UHS 2025-26 prospectus, examining three primary dimensions:

- **Word Frequency Analysis**: Identification of most frequently occurring words to reveal institutional priorities and dominant themes
- **Descriptive Statistics**: Assessment of word length distribution, vocabulary richness, and document complexity
- **Probability Distribution**: Evaluation of keyword concentration across the 83-page document to ensure balanced thematic coverage

## Methodology

### Data Source

University of Health Sciences 2025-26 Prospectus (83 pages, PDF format)

### Tools and Libraries

- **Python 3.x**: Primary programming language
- **NLTK (Natural Language Toolkit)**: Tokenization, text preprocessing, and stopword removal
- **PyMuPDF (fitz)**: Page-by-page PDF text extraction
- **Pandas**: Data organization and statistical computation
- **NumPy**: Numerical calculations and descriptive statistics
- **Matplotlib**: Data visualization and chart generation
- **Collections.Counter**: Efficient word frequency counting
- **Regular Expressions (re)**: Text cleaning and pattern matching

### Processing Steps

#### Step 1: Text Preprocessing

The raw prospectus text underwent systematic cleaning:

- **Tokenization**: Text broken into individual word tokens
- **Lowercasing**: All characters converted to lowercase for uniform processing
- **Punctuation Removal**: Symbols and special characters stripped to isolate words
- **Whitespace Normalization**: Multiple spaces and newlines standardized to single spaces
- **Number Removal**: Numeric characters excluded from analysis

#### Step 2: Word Frequency Analysis

Frequency distribution calculated using collections.Counter:

- Created comprehensive word frequency dictionary
- Sorted occurrences in descending order
- Extracted top 20 most frequent terms
- Generated distribution visualizations

#### Step 3: Descriptive Statistics

Statistical metrics calculated for vocabulary assessment:

- **Total Word Count**: 21,319 words
- **Unique Words**: 2,976 distinct terms
- **Word Length Metrics**:
  - Mean word length
  - Median word length
  - Standard deviation
  - Minimum and maximum lengths

#### Step 4: Probability Analysis Across Pages

Page-wise keyword distribution evaluated:

- Text extracted separately for each of 83 pages
- Selected keywords tokenized and counted per page
- Probability calculated as: P(word) = (Word count on page) / (Total words on page)
- Probability distributions visualized using line charts

## Key Findings

### Overall Text Statistics

- **Total Words**: 21,319
- **Unique Words**: 2,976
- **Mean Word Frequency**: 7.16
- **Median Word Frequency**: 2.0
- **Maximum Word Frequency**: 1,063 (the word "the")
- **Frequency Standard Deviation**: 35.15

### Most Frequent Words (Top 15)

| Rank | Word | Frequency | Highest Probability Page |
|------|------|-----------|------------------------|
| 1 | the | 1,063 | 57 |
| 2 | of | 823 | 81 |
| 3 | in | 541 | 7 |
| 4 | and | 521 | 25 |
| 5 | ing | 485 | 25 |
| 6 | medical | 439 | 8 |
| 7 | to | 324 | 79 |
| 8 | college | 321 | 8 |
| 9 | for | 306 | 56 |
| 10 | a | 216 | 6 |
| 11 | be | 184 | 70 |
| 12 | pr | 183 | 31 |
| 13 | c | 180 | 55 |
| 14 | punjab | 177 | 8 |
| 15 | dental | 168 | 45 |

### High-Impact Keywords (Domain-Specific)

The following words consistently appeared in admission and regulatory sections:

- **admission**: Central to application and enrollment procedures
- **program**: Academic offerings and curriculum
- **university**: Institutional identity and branding
- **faculty**: Academic staff and expertise
- **session**: Academic calendar and scheduling
- **medical**: Primary institutional focus
- **college**: Specific departments and divisions
- **dental**: Specialized medical program

### Text Complexity Findings

- **Mean Word Length per Page**: Ranges from 1.49 to 2.04 characters (standardized measure)
- **Vocabulary Distribution**: Consistent across pages with minor variations
- **Unique Words per Page**: Average 143 unique words per page out of approximately 257 total words per page
- **Frequency Distribution**: Highly skewed, with small number of words appearing frequently while majority appear rarely

## Analysis and Interpretation

### Document Structure

The UHS prospectus demonstrates consistent formatting with approximately 257 words per page across all 83 pages. This uniform structure suggests deliberate editorial control and professional document design.

### Institutional Emphasis

The prominence of "medical" (439 occurrences) and "college" (321 occurrences) clearly establishes UHS's identity as a medical education institution. The frequency of "program," "faculty," and "admission" reflects the document's primary function: communicating academic offerings and enrollment procedures.

### Keyword Distribution Insights

Analysis of keyword probability across pages reveals:

- **Balanced Distribution**: Most high-frequency words distributed relatively evenly across the document
- **Concentrated Emphasis**: Some keywords show concentrated usage in specific sections (e.g., "admission" peaks at page 34 with 0.074 probability)
- **Uneven Coverage**: Terms like "research" and "innovation" show minimal representation, suggesting potential communication gaps regarding academic research initiatives

### Readability Assessment

The moderate vocabulary complexity (mean word length ~1.8) and consistent structure indicate the prospectus is designed for general audience comprehension. However, the presence of specialized medical terminology may create barriers for non-technical readers.

## Visualizations Generated

1. **Words per Page Distribution**: Bar chart showing 257 words consistently across all 83 pages
2. **Unique Words per Page**: Trend analysis showing vocabulary diversity per page (average 143 unique terms)
3. **Mean Word Frequency Distribution**: Red bar chart showing consistent mean frequency (~1.7) across pages
4. **Word Frequency Distribution**: Histogram of overall word frequency showing characteristic long-tail distribution
5. **Keyword Probability Across Pages**: Multi-line chart tracking "admission," "program," "student," "fee," and "university" across all pages
6. **Highest Page-wise Probability**: Bar chart showing peak probability values for top 15 words

## Technical Skills Demonstrated

- **Natural Language Processing**: Text tokenization, preprocessing, and cleaning
- **Statistical Analysis**: Descriptive statistics, probability calculation, distribution analysis
- **Data Visualization**: Chart generation, multi-series visualization, probability distribution plots
- **Programming**: Python automation, efficient data structures, file I/O operations
- **Data Science**: Feature extraction, quantitative text analysis, interpretation

## Files in Repository

- **final_project.ipynb**: Complete Jupyter notebook with all code, outputs, and explanations
- **statistics_word_analysis_report.pdf**: Full project report (13 pages) with visualizations and detailed findings
- **README.md**: This documentation file

## Limitations

- Analysis restricted to text content; visual design and formatting not assessed
- Automated PDF extraction may not capture all formatting or special characters perfectly
- Frequency analysis measures word occurrence but does not capture semantic meaning or sentiment
- Analysis specific to 2025-26 prospectus; results may differ across years or institutions
- Stopwords (the, of, and, etc.) included in analysis; separate analysis with stopwords removed would provide different perspective

## Future Enhancements

Potential extensions to this analysis include:

- Implementation of stopword removal to focus on domain-specific terminology
- Sentiment analysis to assess tone and messaging effectiveness
- N-gram analysis to identify common phrases and compound terms
- Comparison with prospectuses from other institutions
- Temporal analysis comparing prospectuses across multiple years
- Topic modeling (Latent Dirichlet Allocation) to identify underlying themes
- Named entity recognition to extract institution names, program names, and locations

## Key Recommendations

Based on findings, the following improvements are recommended:

1. **Enhance Research Emphasis**: Increase visibility of research achievements and faculty expertise to project academic depth

2. **Improve Accessibility**: Reduce technical jargon or provide definitions to improve comprehension for general audiences

3. **Strengthen Branding**: Emphasize unique institutional characteristics and competitive advantages through strategic keyword placement

4. **Balanced Messaging**: Ensure equal coverage of academic excellence, student support, career outcomes, and institutional values

5. **Engagement Enhancement**: Incorporate student success stories and testimonials to improve prospective student engagement

## Conclusions

The UHS 2025-26 prospectus effectively communicates its identity as a medical education institution through consistent emphasis on medical programs and college structures. The document demonstrates professional structure and readability standards. However, opportunities exist to strengthen institutional branding by expanding emphasis on research initiatives and faculty expertise, which are underrepresented in the current communication.

The analysis methodology and code provided in this repository can be adapted for textual analysis of other institutional documents or educational materials, making this project a reusable framework for document assessment and institutional communication evaluation.

## Academic Context

**Course**: Statistics for Business Analytics  
**Institution**: COMSATS University Islamabad  
**Student**: Daniyal Nadeem (FA24-BBD-120)  
**Submission Date**: December 4, 2025  
**Document Analyzed**: UHS 2025-26 Prospectus (83 pages)

## Project Applications

This analysis demonstrates competency in:
- Natural Language Processing and text mining
- Statistical analysis and probability assessment
- Python programming and data science workflows
- Data visualization and presentation
- Business intelligence and document analysis
- Educational technology and institutional research

## References

- Bird, S., Klein, E., & Loper, E. (2009). Natural Language Processing with Python. O'Reilly Media.
- McKinney, W. (2010). Data structures for statistical computing in Python. Proceedings of the 9th Python in Science Conference, 51-56.
- Hunter, J. D. (2007). Matplotlib: A 2D graphics environment. Computing in Science & Engineering, 9(3), 90-95.
- DuBay, W. H. (2004). The Principles of Readability. Impact Information.
- University of Health Sciences. (2025). Prospectus 2025-26. Lahore, Pakistan.
- PyMuPDF Documentation. (2024). PyMuPDF 1.24.0 Documentation.

---

*This project represents a comprehensive application of natural language processing and statistical analysis to institutional communication materials, demonstrating practical data science skills in text mining, statistical analysis, and business intelligence.*
