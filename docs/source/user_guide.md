(user_guide)=

# User Guide

```{toctree}
---
hidden: true
---
dataset
model
local_app
```

`flytekit-learn` is an opinionated machine learning framework that makes going from
prototype to production fast and simple. Taking inspiration from web protocols, `flytekit-learn`
asks the question:

> Is it possible to define a standard set of functions/methods for machine learning that can be
> reused in many different contexts, from model training to batch, streaming,
> or event-based prediction?

## `flytekit-learn` Apps

A *`flytekit-learn` app* is composed of two objects: `Dataset` and `Model`. Together,
they expose method decorator entrypoints that serve as the core building blocks of an end-to-end
machine learning application. The following sections will show you how to:

- {ref}`Define a Dataset <dataset>`: specify where to *read* data from and how to *split* it into training and test
  sets, *parse* out features and targets, and *iterate* through batches of data.
- {ref}`Bind a Model and Dataset <model>`: specify how to *initialize*, *train*, *evaluate*, and generate
  *predictions* from a model given a `Dataset`.
- {ref}`Train and Predict Locally <local_app>`: do training and prediction using a `flytekit-learn` as a regular
  python script, then serve a `FastAPI` app for prediction.