# AI Models for Sports Streaming and Match Analysis

## Overview

This project consists of two AI models designed to enhance the user experience in virtual reality environments for sports streaming. The models focus on predicting stream quality and analyzing first-half match statistics to predict the dominant team for the second half of a match.

### Models:

1. **StreamIQ Model**: This model predicts the quality of live stream broadcasts by analyzing network data such as internet speed, packet loss, and frame rate. It classifies stream quality into three categories: `Poor`, `Good`, and `Excellent`.
   
2. **SecondHalf Dominator AI Model**: This model analyzes first-half match statistics (e.g., shots, possession, fouls) to predict which team is likely to dominate the second half of the match.

## Technologies Used

- **StreamIQ Model**:
    - **Random Forest** algorithm was used to train the model and predict stream quality based on network metrics such as speed, latency, and dropped frames.
    - Data collected from Kaggle, containing live stream quality data (speed, latency, and dropped frames).
    - Synthetic data generated for the `stream_quality` column, classifying stream quality into categories like `Poor`, `Good`, and `Excellent`.
    - SMOTE technique used to balance the classes in the dataset.
  
- **SecondHalf Dominator AI Model**:
    - Data from Kaggle, containing first-half match statistics such as shots, possession, fouls, and more.
    - Logistic regression used for classification, predicting which team will dominate the second half based on first-half performance.

## Dataset Details

- **StreamIQ Model**:
    - The dataset contains real-world network data and synthetic stream quality data. The `stream_quality` column is generated based on network metrics and classifies stream quality into `Poor`, `Good`, and `Excellent`.
  
- **SecondHalf Dominator AI Model**:
    - The dataset includes real-world match data from Kaggle, containing first-half statistics like shots, possession, fouls, etc. These statistics are used to predict which team will dominate the second half.

## Model Performance

- **StreamIQ Model**:
    - **Accuracy**: 99.89%
    - The model performs well in predicting stream quality with good balance between precision, recall, and F1-score.

- **SecondHalf Dominator AI Model**:
    - **Accuracy**: 98.25%
    - The model successfully predicts which team is likely to dominate in the second half based on first-half match statistics.

## How to Use the Demo (SecondHalf Dominator AI)

1. **Choose a Match**:
    - Select a match for which you want to predict the dominant team based on first-half statistics.

2. **Analyze First Half**:
    - The model takes first-half statistics such as shots, possession, fouls, etc.

3. **Prediction Output**:
    - The AI predicts which team is likely to dominate the second half based on first-half performance.

4. **Interactive Interface**:
    - The demo provides visual outputs (charts) comparing the teams’ first-half performance, with predictions for the second half.

## Conclusion

These AI models enhance the sports streaming experience in virtual environments. StreamIQ improves stream quality, while SecondHalf Dominator AI provides insightful predictions based on first-half match data. Both models deliver high accuracy and offer interactive features for users in real-time sports events.
# ملاحظات هامة حول الملفات والمودلين:

### مشكلة في فتح ملف  (SecondHalf_Dominator_AI_model.ipynb)

قد يواجه المستخدمون مشكلة في فتح ملف SecondHalf_Dominator_AI_model.ipynb مباشرة على GitHub بسبب بعض المشاكل المتعلقة بالمكتبة الخاصة بالديمو. لذا، لحل هذه المشكلة، يرجى اتباع الخطوات التالية:

1. تنزيل الملف على جهازك:
   - قم بتنزيل ملف من الخانه الجانبيه SecondHalf_Dominator_AI_model.ipynb على جهازك.

2. فتح الملف باستخدام Google Colab:
   - بعد تنزيل الملف، قم بفتح Google Colab [من هنا](https://colab.research.google.com/).
   - قم بتحميل الملف الذي قمت بتنزيله باستخدام خيار "فتح ملف من جهازك".
   - سيتمكن المستخدم من تشغيل الملف وتنفيذ الأكواد الخاصة بالنموذج.

### ملاحظات إضافية:
- نسخة Python (.py): تم أيضًا إضافة نسخة من النموذج بلغة Python ضمن الملفات المرفقة، يمكنك استخدامها بدلاً من الملف السابق 
  
- مجلد البيانات المضغوط: تم إضافة مجلد مضغوط يحتوي على الداتا سيت التي تم استخدامها في النموذجين. يمكنك فك الضغط واستخدام البيانات لتشغيل النماذج بشكل صحيح.
