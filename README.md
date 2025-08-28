# Swiggy_Delivery_Time_Predictor_11 CaseCraft Analytics Project Sprint Project 11


## 🍽️ Overview  
This project models Swiggy’s food delivery time using synthetic order, location, and traffic data. It combines geospatial features, temporal patterns, and regression modeling to estimate delivery duration and optimize logistics.

## 🎯 Objective  
To predict delivery time per order using distance, order size, time of day, and traffic level—supporting operational planning and customer experience.

## 📦 Dataset & Features  
- Orders: 1,000 synthetic deliveries  
- Features:  
  - Restaurant & customer coordinates  
  - Order size (1–5 items)  
  - Time of day (Morning, Afternoon, Evening, Night)  
  - Traffic level (Low, Medium, High)  
  - Distance (km)  
- Target: `delivery_time_min` (continuous)

## 📊 Visual Explorations  
- Histogram: Delivery time distribution  
- Scatterplot: Distance vs Delivery time (colored by traffic)  
- Boxplot: Delivery time by time of day  
- Scatterplot: Predicted vs Actual delivery time  
- Heatmap: Confusion matrix (binned delivery time)

## 🤖 Predictive Modeling  
- Model: Random Forest Regressor  
- Encoded features: time of day, traffic level  
- Performance:  
  - Mean Absolute Error: **1.80 minutes**  
  - Strong bin-level accuracy in confusion matrix

## 🧠 Key Insights  
1. **Distance & Traffic**: Strong predictors of delivery time  
2. **Time of Day Impact**: Evening and night orders show higher variability  
3. **Model Accuracy**: MAE under 2 minutes on synthetic data  
4. **Operational Levers**: Traffic and time-of-day can guide delivery estimates  
5. **Customer Experience**: Binned predictions help set realistic expectations

## ✅ Final Conclusion  
Swiggy can leverage predictive modeling to estimate delivery time with high accuracy. This framework supports logistics optimization, dynamic ETAs, and customer satisfaction—especially when factoring in traffic and time-of-day effects.