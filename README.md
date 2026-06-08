<div align="center">
<h1>AWS AI &amp; ML Scholars</h1>
</div>

# Context

- [Context](#context)
- [Introduction](#introduction)
- [ML Fundamentals](#ml-fundamentals)
  - [Training data](#training-data)
    - [Labeled data](#labeled-data)
    - [Unlabeled data](#unlabeled-data)
    - [Structured data](#structured-data)
    - [Unstructured data](#unstructured-data)
  - [Machine Learning Process](#machine-learning-process)
  - [Inferencing](#inferencing)
    - [Batch Inferencing](#batch-inferencing)
    - [Real-time Inferencing](#real-time-inferencing)

# Introduction

- **AI vs. ML:** AI is the broader field; ML is one way to achieve it
- **Core vocabulary:** introduces key terms you’ll use throughout the course
- **Real-world uses:** shows how AI and ML appear in practical applications
- **Foundational focus:** builds a basic mental model before deeper topics

- Venn Diagram

  ![venn diagram](https://i.imgur.com/vYGuEJM.png)

  - **Artificial intelligence (AI)**

    AI is a broad field that encompasses the development of intelligent systems capable of performing tasks that typically require human intelligence, such as perception, reasoning, learning, problem-solving, and decision-making. AI serves as an umbrella term for various techniques and approaches, including machine learning, deep learning, and generative AI, among others.
  - **Machine learning (ML)**

    ML is a type of AI for understanding and building methods that make it possible for machines to learn. These methods use data to improve computer performance on a set of tasks.

  - **Deep learning (DL)**

    Deep learning uses the concept of neurons and synapses similar to how our brain is wired. An example of a deep learning application is Amazon Rekognition, which can analyze millions of images and streaming and stored videos within seconds.

  - **Generative AI**

    Generative AI is a subset of deep learning because it can adapt models built using deep learning, but without retraining or fine tuning.

    Generative AI systems are capable of generating new data based on the patterns and structures learned from training data.

---
[⬆️ Go to Context](#context)

# ML Fundamentals

- Building a machine learning model involves data collection and preparation, selecting an appropriate algorithm, training the model on the prepared data, and evaluating its performance through testing and iteration.
- The machine learning process starts with collecting and processing training data. Bad data is often called garbage in, garbage out, and therefore an ML model is only as good as the data used to train it. Although data preparation and processing are sometimes a routine process, it is arguably the most critical stage in making the whole model work as intended or ruining its performance.
- There are a several different types of data used in training an ML model. First, it's important to know the difference between **labeled** and **unlabeled** data.

---
[⬆️ Go to Context](#context)

## Training data

---
[⬆️ Go to Context](#context)

### Labeled data

- Labeled data is a dataset where each instance or example is accompanied by a label or target variable that represents the desired output or classification. These labels are typically provided by human experts or obtained through a reliable process.
- *Example:* In an image classification task, labeled data would consist of images along with their corresponding class labels (for example, cat, dog, car).

---
[⬆️ Go to Context](#context)

### Unlabeled data

- Unlabeled data is a dataset where the instances or examples do not have any associated labels or target variables. The data consists only of input features, without any corresponding output or classification.
- *Example:* A collection of images without any labels or annotations

---
[⬆️ Go to Context](#context)

The main types of data used in training are structured and unstructured data. They come with various subtypes, which you can find by expanding the following categories.

### Structured data

- Structured data refers to data that is organized and formatted in a predefined manner, typically in the form of tables or databases with rows and columns. This type of data is suitable for traditional machine learning algorithms that require well-defined features and labels. The following are types of structured data.
- **Tabular data:** This includes data stored in spreadsheets, databases, or CSV files, with rows representing instances and columns representing features or attributes.
- **Time-series data:** This type of data consists of sequences of values measured at successive points in time, such as stock prices, sensor readings, or weather data.

---
[⬆️ Go to Context](#context)

### Unstructured data

- Unstructured data is data that lacks a predefined structure or format, such as text, images, audio, and video. This type of data requires more advanced machine learning techniques to extract meaningful patterns and insights.
- **Text data:** This includes documents, articles, social media posts, and other textual data.
- **Image data:** This includes digital images, photographs, and video frames.

---
[⬆️ Go to Context](#context)

## Machine Learning Process

- ML process

  ![ml process](https://i.imgur.com/qwbSo4e.png)

- The compiled training data is fed into machine learning algorithms. The ML learning process is traditionally divided into three broad categories: supervised learning, unsupervised learning, and reinforcement learning.

- Supervised Learning
  - In supervised learning, the algorithms are trained on labeled data. The goal is to learn a mapping function that can predict the output for new, unseen input data.
- Unsupervised Learning
  - It is refers to algorithms that learn from unlabeled data. The goal is to discover inherent patterns, structures, or relationships within the input data.
- Reinforcement Learning
  - In reinforcement learning, the machine is given only a performance score as guidance and semi-supervised learning, where only a portion of training data is labeled. Feedback is provided in the form of rewards or penalties for its actions, and the machine learns from this feedback to improve its decision-making over time.

---
[⬆️ Go to Context](#context)

## Inferencing

- After the model has been trained, it is time to begin the process of using the information that a model has learned to make predictions or decisions. This is called inferencing.
- There are two main types of inferencing in machine learning: **batch inferencing** and **real-time inferencing**.

---
[⬆️ Go to Context](#context)

### Batch Inferencing

- Batch inferencing is when the computer takes a large amount of data, such as images or text, and analyzes it all at once to provide a set of results. This type of inferencing is often used for tasks like data analysis, where the speed of the decision-making process is not as crucial as the accuracy of the results.

---
[⬆️ Go to Context](#context)

### Real-time Inferencing

- Real-time inferencing is when the computer has to make decisions quickly, in response to new information as it comes in. This is important for applications where immediate decision-making is critical, such as in chatbots or self-driving cars. The computer has to process the incoming data and make a decision almost instantaneously, without taking the time to analyze a large dataset.

---
[⬆️ Go to Context](#context)
