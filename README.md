# Unit-3: Data Wrangling (Experiment 15)

## Author Information
* **Name:** RUDRANSH SHARMA
* **PRN:** 25070123096

## AIM
To study different data normalization techniques and encoding methods in Pandas and Scikit-learn for converting categorical data into numerical form.

## THEORY
The following functions and concepts are utilized for data scaling and feature encoding:

* **`pd.DataFrame()`**: Creates a structured tabular dataset from dictionary data.
* **`print()`**: Displays output on the console.
* **`df['col'].min()`**: Returns the minimum value in a column.
* **`df['col'].max()`**: Returns the maximum value in a column.
* **Min-Max Normalization**: Scales values between 0 and 1 using the formula: `(x - min) / (max - min)`.
* **`df[cols]`**: Selects multiple columns from a DataFrame for simultaneous processing.
* **`df.mean()`**: Calculates the average value of a column.
* **`df.std()`**: Calculates the standard deviation of a column.
* **Z-Score Normalization**: Standardizes data by centering it around a mean of 0 with a standard deviation of 1 using `(x - mean) / std`.
* **Decimal Scaling**: Normalizes data by dividing values by a power of 10 to move the decimal point.
* **`display()`**: Shows the DataFrame in a formatted tabular layout.
* **`pd.read_csv()`**: Loads an external dataset from a CSV file into a DataFrame.
* **`LabelEncoder()`**: A Scikit-learn tool that converts categorical labels into a sequence of integers.
* **`fit_transform()`**: A method that fits the encoder to the data and then transforms it into numeric form in one step.
* **`pd.get_dummies()`**: Converts categorical variables into "One-Hot" encoded columns (binary columns for each category).
* **`drop_first=True`**: Removes one dummy column to prevent multicollinearity (the "dummy variable trap").
* **Normalization on multiple columns**: Applying scaling operations on a selection of numerical features together.
* **Categorical to numerical conversion**: A critical preprocessing step required for machine learning models to process non-numeric data.

## ALGORITHM
The logical workflow for preprocessing through normalization and encoding is as follows:

1.  **Data Acquisition**: Load or create a dataset containing a mix of numerical features and categorical strings.
2.  **Numerical Scaling (Normalization)**:
    * **Min-Max**: Apply range scaling to bring features into a [0, 1] interval.
    * **Standardization**: Apply Z-Score scaling to ensure features have a Gaussian distribution properties.
    * **Decimal Scaling**: Scale by powers of 10 based on the maximum absolute value in the feature.
3.  **Label Encoding**: Assign a unique integer to each category in ordinal or target columns using `LabelEncoder`.
4.  **One-Hot Encoding**: Transform nominal categorical variables into separate binary columns using `get_dummies` to avoid implying a false mathematical order.
5.  **Integration**: Replace the original raw features with the normalized and encoded numerical representations.

## CONCLUSION
In this experiment, we studied different normalization techniques such as Min-Max, Z-score,
