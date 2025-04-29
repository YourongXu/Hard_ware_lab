### Discussion

#### 1. Play with your sorting hat. Are all 10 questions important to create the sorting hat? If you were to remove some questions to improve user experience, which questions would you remove and justify your answer.

Not all questions are equally important. According to the decision tree, each question has a feature importance score. The higher the score, the more it influences the final classification result. Questions with lower scores contribute less and can potentially be removed to improve user experience without significantly reducing model accuracy.



#### 2. If you were to improve the sorting hat, what technical improvements would you make? Consider:

- How could you improve the model's accuracy or efficiency?  
  I would collect more base data and remove less important questions to improve both accuracy and model efficiency.

- What additional sensors or hardware could enhance the user experience?  
  I would add a microphone and use voice recognition so users can speak their answers instead of pressing buttons.

- Does decision tree remain suitable for your choice of new sensors? If yes, carefully justify your answer. If not, what ML model would you use and explain why.  
  A decision tree may no longer be suitable. It works best with discrete, structured data. However, if we introduce continuous or high-dimensional data like speech or motion, its performance may degrade. In that case, I would consider a lightweight neural network (e.g., 1D CNN), which is better suited for processing time-series data like voice or movement.
