# INN Hotels – Booking Cancellation Risk Model

**Type:** Classification  
**Tools:** Python, scikit-learn, Pandas, NumPy

## Problem
INN Hotels faced significant revenue loss from unpredictable booking cancellations with no system to identify high-risk reservations in advance.

## Approach
Built and compared logistic regression and decision tree classifiers on 36,275 bookings. Engineered features from lead time, room type, meal plan, market segment, and special requests. Split data 70/30 for training and evaluation.

## Results
| Model | Accuracy | 
|-------|----------|
| Logistic Regression | ~75% |
| Decision Tree | ~78% |

## Key Findings
- 32.8% overall cancellation rate — a significant revenue risk
- Canceled bookings averaged 139-day lead time vs. 59 days for kept bookings
- Customers who canceled made far fewer special requests (0.33 avg vs. 0.76)
- Online bookings had the highest cancellation rate at 36.5%
- July had the highest monthly cancellation rate at 45%

## Recommendations
- Flag bookings with lead times over 100 days as high cancellation risk
- Implement stricter cancellation policies during summer months
- Prompt customers to make special requests at booking — strongly tied to retention
- Consider overbooking strategies for Room Type 6 (42% cancellation rate)

## Files
| File | Description |
|------|-------------|
| `INN_Hotels.ipynb` | Full modeling notebook |
| `INNHotelsGroup.csv` | Raw dataset |
