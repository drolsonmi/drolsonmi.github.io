## Lecture 1: The Machine Learning Landscape - 7 Jan 2026

* Intro to course
* Writing Reports for projects

## Lecture 2: The Machine Learning Process - 9 Jan 2026

[Demo of the Machine Learning Process - Google CoLab Example](https://colab.research.google.com/drive/1aVvjaLiGBBRe7sKE31ODkb9NGQ1Adjfh?usp=drive_link)

## Lecture 3: Preprocessing - 12 Jan 2026
* What is EDA? Goals of EDA
* Preprocessing
    > ```python
    > sns.load_dataset('Titanic')`
    > ```
    > 
    > What needs to be done to this dataset?
    > * Remove columns
    >     * 'embarked' (repeat of 'embark_town')
    >     * 'class' (repeat of 'pclass')
    >     * 'alive' (repeat of 'survived')
    >     * 'adult_male' (more or less repeat of 'who')
    > * Missing values
    >     * Remove 'deck' column
    >     * 'age' column - fill average based on 'class' and 'who'
    > * Encode
    >     * 'sex' - Binary encoding (can do as ordinal)
    >     * 'who' - One-hot encoding (`pd.GetDummies`)
    >     * 'embark_town' - One-hot encoding
    >     * 'alone' - Binary encoding

## Lecture 4: Preprocessing - 14 Jan 2026
* Finish preprocessing
* Feature Scaling
* Piping
* scikit-learn

> Students try some preprocessing with the `diamonds` dataset in *seaborn*