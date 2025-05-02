# CPE393-model-monitoring (References)

https://github.com/evidentlyai/ml_observability_course

https://www.analyticsvidhya.com/blog/2024/03/complete-guide-to-effortless-ml-monitoring-with-evidently-ai/

https://fullstackdeeplearning.com/course/2022/lecture-6-continual-learning/


# Data Drift Report Summary

- **Total Tests:** 644  
- **Tests Passed:** 643  
- **Warnings:** 0  
- **Failed Tests:** 1  
- **Errors:** 0  

## Summary

- Only 1 test failed out of 644. This means the data is very stable.
- The amount of drifted columns is very small: only 1 out of 643 columns (about 0.16%).
- This is much lower than the alert level of 30%, so it is not a problem.

## Details

- The drift check used the Jensen-Shannon distance method.
- Example columns like `Dest_MGM`, `Origin_BRO`, and `Dest_SPS` had very low drift scores.
- These scores were much lower than the threshold of 0.1, so they passed.

## Conclusion

The data is stable and has no major drift can keep using it safely.
