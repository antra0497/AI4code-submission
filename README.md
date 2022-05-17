# AI4code-submission

#### Welcome to the Google AI4Code Competition!

In this competition you're challenged to reconstruct the order of Kaggle notebooks whose cells have been shuffled. Check out the Competition Pages for a complete overview.

This notebook will walk you through making a submission with a simple ranking model. We'll look at how to:

Wrangle the competition data and create validation splits,
Represent the code cell orders with a feature,
Build a ranking model with XGBoost,
Evaluate predictions with a Python implementation of the competition metric, and,
Format predictions to make a successful submission.
Our model will be able to learn roughly where a cell should go in a notebook based on what words it contains -- that, for example, cells containing "Introduction" or import should usually be near the beginning, while cells containing "Submit" or submission.csv should usually be near the end. These simple features are effective at reconstructing the global order of typical data science workflows. An understanding of the interactions or relationships between cells, however, will be required of the most successful solutions.
