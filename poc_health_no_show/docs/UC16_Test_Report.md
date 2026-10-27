| Test                         | Expected result            | Actual result | Status    |
| ---------------------------- | -------------------------- | ------------- | --------- |
| Bronze row count             | 110,527                    |  110,527      | Pass/Fail |
| No duplicate appointment IDs | 0 duplicates               |  0 duplicates | Pass/Fail |
| No invalid ages              | 0 rows                     |  1 rows       | Pass/Fail |
| No invalid date sequence     | 0 rows                     |               | Pass/Fail |
| Risk segment thresholds      | 0 mismatches               |               | Pass/Fail |
| High-risk no-show rate       | Higher than lower segments |               | Pass/Fail |
| AI messages generated        | No null/empty messages     |               | Pass/Fail |
| Unsafe AI content            | 0 unsafe messages          |               | Pass/Fail |
| Genie answers demo questions | Correct and safe           |               | Pass/Fail |