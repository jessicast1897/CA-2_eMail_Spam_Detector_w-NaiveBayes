# CA-2_Spam_Email_Detector
using a set of emails to train a learning model to detect spam email. 

- Emails in each folder are randomly mixed.
- **Spam emails** are identified by file names that begin with `spmsg`.
- **Non-spam emails** follow a numeric naming convention.

---

## Approach
The solution uses a **Bag-of-Words** representation to convert emails into numerical feature vectors.

### High-Level Steps
1. Read and preprocess all training emails.
2. Remove non-alphabetic tokens and single-character words.
3. Build a vocabulary using the **3000 most frequent words** from the training set.
4. Convert each email into a feature vector based on word counts.
5. Assign labels using file name conventions.
6. Train a **Multinomial Naive Bayes** classifier.
7. Evaluate performance on the test dataset using **classification accuracy**.

---

## Files Included
- **CA02_NB_assignment.ipynb** – Main notebook containing the implementation and explanations  
- **README.md** – Project overview and execution instructions  
- **train-mails/** – Training email dataset  
- **test-mails/** – Testing email dataset  

---

## How to Run
1. Place the notebook and the `train-mails` and `test-mails` folders in the same directory.
2. Open `CA02_NB_assignment.ipynb`.
3. Run all cells from top to bottom.
4. The final cell will print the classification accuracy on the test dataset.

---

## Notes
- The model uses **word count features** and does not consider word order or semantic context.
- **Accuracy** is reported as the primary evaluation metric.
- The implementation is modularized to separate:
  - Vocabulary creation  
  - Feature extraction  
  - Model training  
  - Model evaluation  

---

## Author
**Jessica Shono Thai and Bhavna Sreekumar 
