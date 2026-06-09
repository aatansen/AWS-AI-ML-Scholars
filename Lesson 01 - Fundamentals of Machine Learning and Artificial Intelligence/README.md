<div align="center">
<h1>Fundamentals of Machine Learning and Artificial Intelligence</h1>
</div>

# **Context**

- [**Context**](#context)
- [**Introduction**](#introduction)
- [**ML Fundamentals**](#ml-fundamentals)
  - [Training Data](#training-data)
    - [Labeled Data](#labeled-data)
    - [Unlabeled Data](#unlabeled-data)
    - [Structured Data](#structured-data)
    - [Unstructured Data](#unstructured-data)
  - [Machine Learning Process](#machine-learning-process)
  - [Inferencing](#inferencing)
    - [Batch Inferencing](#batch-inferencing)
    - [Real-time Inferencing](#real-time-inferencing)
- [**Deep Learning Fundamentals**](#deep-learning-fundamentals)
  - [Neural Networks](#neural-networks)
- [**Generative AI Fundamentals**](#generative-ai-fundamentals)
  - [Foundation Models](#foundation-models)
  - [Large Language Models](#large-language-models)
  - [Diffusion Models](#diffusion-models)
  - [Multimodal Models](#multimodal-models)
  - [Other Generative Models](#other-generative-models)
- [**Optimizing Model Outputs**](#optimizing-model-outputs)
  - [Prompt Engineering](#prompt-engineering)
  - [Fine-tuning](#fine-tuning)
  - [Retrieval-augmented Generation](#retrieval-augmented-generation)
- [**QnA on Introduction**](#qna-on-introduction)
- [**AWS Infrastructure and Technologies**](#aws-infrastructure-and-technologies)
  - [ML frameworks](#ml-frameworks)
  - [AI/ML services](#aiml-services)
  - [Generative AI](#generative-ai)
- [**QnA on AWS Services**](#qna-on-aws-services)

# **Introduction**

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

# **ML Fundamentals**

- Building a machine learning model involves data collection and preparation, selecting an appropriate algorithm, training the model on the prepared data, and evaluating its performance through testing and iteration.
- The machine learning process starts with collecting and processing training data. Bad data is often called garbage in, garbage out, and therefore an ML model is only as good as the data used to train it. Although data preparation and processing are sometimes a routine process, it is arguably the most critical stage in making the whole model work as intended or ruining its performance.
- There are a several different types of data used in training an ML model. First, it's important to know the difference between **labeled** and **unlabeled** data.

---
[⬆️ Go to Context](#context)

## Training Data

### Labeled Data

- Labeled data is a dataset where each instance or example is accompanied by a label or target variable that represents the desired output or classification. These labels are typically provided by human experts or obtained through a reliable process.
- *Example:* In an image classification task, labeled data would consist of images along with their corresponding class labels (for example, cat, dog, car).

---
[⬆️ Go to Context](#context)

### Unlabeled Data

- Unlabeled data is a dataset where the instances or examples do not have any associated labels or target variables. The data consists only of input features, without any corresponding output or classification.
- *Example:* A collection of images without any labels or annotations

---
[⬆️ Go to Context](#context)

The main types of data used in training are structured and unstructured data. They come with various subtypes, which you can find by expanding the following categories.

### Structured Data

- Structured data refers to data that is organized and formatted in a predefined manner, typically in the form of tables or databases with rows and columns. This type of data is suitable for traditional machine learning algorithms that require well-defined features and labels. The following are types of structured data.
- **Tabular data:** This includes data stored in spreadsheets, databases, or CSV files, with rows representing instances and columns representing features or attributes.
- **Time-series data:** This type of data consists of sequences of values measured at successive points in time, such as stock prices, sensor readings, or weather data.

---
[⬆️ Go to Context](#context)

### Unstructured Data

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

# **Deep Learning Fundamentals**

The field of deep learning is inspired by the structure and function of the brain. It involves the use of artificial neural networks, which are computational models that are designed to mimic the way the human brain processes information.

---
[⬆️ Go to Context](#context)

## Neural Networks

At the core of deep learning are neural networks. Just like our brains have neurons that are connected to each other, neural networks have lots of tiny units called nodes that are connected together. These nodes are organized into layers. The layers include an input layer, one or more hidden layers, and an output layer.

![Neural networks](https://i.imgur.com/L1w9nkY.png)

> [!NOTE]
>
> - When we show a neural network many examples, like data about customers who bought certain products or used certain services, it figures out how to identify patterns by adjusting the connections between its nodes. It's like the nodes are talking to each other and slowly figuring out the patterns that separate different types of customers.

When a neural network learns to recognize these patterns from the examples, it can then look at data for completely new customers that it has never seen before and still make predictions about what they might buy or how they might behave.

- The following are a couple branches of AI where deep learning is used to enhance results.
  - **Computer vision**

    Computer vision is a field of artificial intelligence that makes it possible for computers to interpret and understand digital images and videos. Deep learning has revolutionized computer vision by providing powerful techniques for tasks such as image classification, object detection, and image segmentation.

  - **Natural language processing (NLP)**

    Natural language processing (NLP) is a branch of artificial intelligence that deals with the interaction between computers and human languages. Deep learning has made significant strides in NLP, making possible tasks such as text classification, sentiment analysis, machine translation, and language generation.

---
[⬆️ Go to Context](#context)

# **Generative AI Fundamentals**

Machine learning has been around for decades, which begs the question, what has led to the emergence of generative AI right now? The answer is as straightforward as huge investments in resources. Hiring a large team, spending on compute resources, and importantly, having the willingness to invest and develop big ideas, are all contributors to the rise of generative AI.

---
[⬆️ Go to Context](#context)

## Foundation Models

![Foundation models](https://i.imgur.com/Dbv6tb8.png)

Generative AI is powered by models that are pretrained on internet-scale data, and these models are called foundation models (FMs).  With FMs, instead of gathering labeled data for each model and training multiple models as in traditional ML, you can adapt a single FM to perform multiple tasks. These tasks include text generation, text summarization, information extraction, image generation, chatbot interactions, and question answering. FMs can also serve as the starting point for developing more specialized models.

**FM lifecycle:** The foundation model lifecycle is a comprehensive process that involves several stages, each playing a crucial role in developing and deploying effective and reliable foundation models.

- **Data selection:** Unlabeled data can be used at scale for pre-training because it is much easier to obtain compared to labeled data. Unlabeled data includes raw data, such as images, text files, or videos, with no meaningful informative labels to provide context. FMs require training on massive datasets from diverse sources.
- **Pre-training:** Although traditional ML models rely on supervised, unsupervised, or reinforcement learning patterns, FMs are typically pre-trained through self-supervised learning. With self-supervised learning, labeled examples are not required. Self-supervised learning makes use of the structure within the data to autogenerate labels.

  During the initial pre-training stage, the FM's algorithm can learn the meaning, context, and relationship of the words in the datasets. For example, the model might learn whether drink means beverage, the noun, or swallowing the liquid, the verb.

  After the initial pre-training, the model can be further pre-trained on additional data. This is known as continuous pre-training. The goal is to expand the model's knowledge base and improve its ability to understand and generalize across different domains or tasks.
- **Optimization:** Pre-trained language models can be optimized through techniques like prompt engineering, retrieval-augmented generation (RAG), and fine-tuning on task-specific data. These methods will vary in complexity and cost and will be discussed later in this lesson.
- **Evaluation:** Whether or not you fine-tune a model or use a pre-trained model off the shelf, the next logical step is to evaluate the model. An FM's performance can be measured using appropriate metrics and benchmarks. Evaluation of model performance and its ability to meet business needs is important.
- **Deployment:** When the FM meets the desired performance criteria, it can be deployed in the target production environment. Deployment can involve integrating the model into applications, APIs, or other software systems.
- **Feedback and continuous improvement:** After deployment, the model's performance is continuously monitored, and feedback is collected from users, domain experts, or other stakeholders. This feedback, along with model monitoring data, is used to identify areas for improvement, detect potential biases or drift, and inform future iterations of the model. The feedback loop permits continuous enhancement of the foundation model through fine-tuning, continuous pre-training, or re-training, as needed.
- **Summary:** It's important to note that the FM lifecycle is an iterative process, where lessons learned and insights gained from each stage can inform and improve subsequent iterations.

> [!NOTE]
>
> - Amazon Bedrock provides access to a choice of high-performing FMs from leading AI companies like AI21 Labs, Anthropic, Cohere, Meta, Mistral AI, Stability AI, and Amazon.
> - With these FMs as a foundation, you can further optimize their outputs with prompt engineering, fine-tuning, or RAG.

---
[⬆️ Go to Context](#context)

## Large Language Models

- Large language models (LLMs) can be based on a variety of architectures, but the most common architecture in today's state-of-the-art models is the transformer architecture. Transformer-based LLMs are powerful models that can understand and generate human-like text. They are trained on vast amounts of text data from the internet, books, and other sources, and learn patterns and relationships between words and phrases.

- **Tokens**
  - Tokens are the basic units of text that the model processes. Tokens can be words, phrases, or individual characters like a period. Tokens also provide standardization of input data, which makes it easier for the model to process.
  - As an example, the sentence "A puppy is to dog as a kitten is to cat." might be broken up into the following tokens: “A” “puppy” “is” “to” “dog” “as” "a" “kitten” “is” “to” "cat."

    ![token](https://i.imgur.com/bpYdYwx.png)

- **Embeddings and vectors**
  - Embeddings are numerical representations of tokens, where each token is assigned a vector (a list of numbers) that captures its meaning and relationships with other tokens. These vectors are learned during the training process and allow the model to understand the context and nuances of language.
  - For example, the embedding vector for the token "cat" might be close to the vectors for "feline" and "kitten" in the embedding space, indicating that they are semantically related. This way, the model can understand that "cat" is similar to "feline" and "kitten" without being explicitly programmed with those relationships.

    ![Embeddings and vectors](https://i.imgur.com/i6mtfOi.png)

> [!NOTE]
>
> - LLMs use these tokens, embeddings, and vectors to understand and generate text. The models can capture complex relationships in language, so they can generate coherent and contextually appropriate text, answer questions, summarize information, and even engage in creative writing.

---
[⬆️ Go to Context](#context)

## Diffusion Models

Diffusion is a deep learning architecture system that starts with pure noise or random data. The models gradually add more and more meaningful information to this noise until they end up with a clear and coherent output, like an image or a piece of text. Diffusion models learn through a two-step process of forward diffusion and reverse diffusion.

- **Forward diffusion:** Using forward diffusion, the system gradually introduces a small amount of noise to an input image until only the noise is left over.

  ![Forward diffusion](https://i.imgur.com/p3pWSdV.png)

- **Reverse diffusion:** In the subsequent reverse diffusion step, the noisy image is gradually introduced to de-noising until a new image is generated.

  ![Reverse diffusion](https://i.imgur.com/oaPGh2P.png)

> [!NOTE]
>
> - Although some of the most well-known and impressive applications of diffusion models have been text-to-image models, diffusion models can be applied to a variety of tasks beyond just image generation.

---
[⬆️ Go to Context](#context)

## Multimodal Models

- Instead of just relying on a single type of input or output, like text or images, multimodal models can process and generate multiple modes of data simultaneously. For example, a multimodal model could take in an image and some text as input, and then generate a new image and a caption describing it as output.

- These kinds of models learn how different modalities like images and text are connected and can influence each other. Multimodal models can be used for automating video captioning, creating graphics from text instructions, answering questions more intelligently by combining text and visual info, and even translating content while keeping relevant visuals.

---
[⬆️ Go to Context](#context)

## Other Generative Models

There are several types of generative models used in ML and AI.

- **Generative adversarial networks (GANs)**
  - GANs are a type of generative model that involves two neural networks competing against each other in a zero-sum game framework. The two networks are generator and discriminator.
  - Generator: This network generates new synthetic data (for example, images, text, or audio) by taking random noise as input and transforming it into data that resembles the training data distribution.
  - Discriminator: This network takes real data from the training set and synthetic data generated by the generator as input. Its goal is to distinguish between the real and generated data.
  - During training, the generator tries to generate data that can fool the discriminator into thinking it's real, while the discriminator tries to correctly classify the real and generated data. This adversarial process continues until the generator produces data that is indistinguishable from the real data.

- **Variational autoencoders (VAEs)**
  - VAEs are a type of generative model that combines ideas from autoencoders (a type of neural network) and variational inference (a technique from Bayesian statistics). In a VAE, the model consists of two parts:
  - Encoder: This neural network takes the input data (for example, an image) and maps it to a lower-dimensional latent space, which captures the essential features of the data.
  - Decoder: This neural network takes the latent representation from the encoder and generates a reconstruction of the original input data.
  - The key aspect of VAEs is that the latent space is encouraged to follow a specific probability distribution (usually a Gaussian distribution), which allows for generating new data by sampling from this latent space and passing the samples through the decoder.

---
[⬆️ Go to Context](#context)

# **Optimizing Model Outputs**

A key part of the foundation model lifecycle is the optimization phase. An FM can be further optimized in several different ways. These techniques vary in complexity and cost, with the fastest and lowest cost option being prompt engineering.

## Prompt Engineering

Prompts act as instructions for foundation models. Prompt engineering focuses on developing, designing, and optimizing prompts to enhance the output of FMs for your needs. It gives you a way to guide the model's behavior to the outcomes that you want to achieve.

A prompt's form depends on the task that you are giving to a model. As you explore prompt engineering examples, you will review prompts containing some or all of the following elements:

- Instructions: This is a task for the FM to do. It provides a task description or instruction for how the model should perform.
- Context: This is external information to guide the model.
- Input data: This is the input for which you want a response.
- Output indicator: This is the output type or format.

*Example prompt*:
You are an experienced journalist that excels at condensing long articles into concise summaries. Summarize the following text in 2–3 sentences.
Text: [Long article text goes here]

## Fine-tuning

Although FMs are pre-trained through self-supervised learning and have inherent capability of understanding information, fine-tuning the FM base model can improve performance. Fine-tuning is a supervised learning process that involves taking a pre-trained model and adding specific, smaller datasets. Adding these narrower datasets modifies the weights of the data to better align with the task.

There are two ways to fine-tune a model:

- **Instruction fine-tuning:** It uses examples of how the model should respond to a specific instruction. Prompt tuning is a type of instruction fine-tuning.
- **Reinforcement learning from human feedback (RLHF):** It provides human feedback data, resulting in a model that is better aligned with human preferences.

*Consider this use case for fine-tuning:* If you are working on a task that requires industry knowledge, you can take a pre-trained model and fine-tune the model with industry data. If the task involves medical research, for example, the pre-trained model can be fine-tuned with articles from medical journals to achieve more contextualized results.

## Retrieval-augmented Generation

**Retrieval-augmented generation (RAG)** is a technique that supplies domain-relevant data as context to produce responses based on that data. This technique is similar to fine-tuning. However, rather than having to fine-tune an FM with a small set of labeled examples, RAG retrieves a small set of relevant documents and uses that to provide context to answer the user prompt. RAG will not change the weights of the foundation model, whereas fine-tuning will change model weights.

---
[⬆️ Go to Context](#context)

# **QnA on Introduction**

1. A company wants to develop a system that can accurately recognize and classify handwritten digits from images.Which of the following options best describes the use of neural networks for this task?
   - [ ] Neural networks are a type of decision tree algorithm that can be trained on image data to create a set of rules for classifying handwritten digits.
   - [ ] Neural networks are a form of linear regression that can be used to map pixel values from images to corresponding digit labels.
   - [x] Neural networks are a type of deep learning model inspired by the structure and function of the human brain. They consist of interconnected nodes that can learn to recognize patterns in data, such as images of handwritten digits.
   - [ ] Neural networks are a type of database system that can store and retrieve images of handwritten digits based on their pixel values and associated labels.

2. A company is developing an artificial intelligence (AI) system to control a self-driving car. The system learns through trial-and-error interactions with the driving environment, receiving rewards for safe and efficient actions. Which machine learning (ML) approach is being used in this scenario?
   - [ ] Supervised learning
   - [x] Reinforcement learning
   - [ ] Unsupervised learning
   - [ ] Self-supervised learning

3. A company is developing a large language model (LLM) for natural language processing tasks, such as text generation, summarization, and question answering.Which of the following best describes the role of embeddings, in the context of LLMs?
   - [x] Embeddings are numerical representations of words or tokens, where semantically similar words have similar vector representations.
   - [ ] Embeddings are the preprocessing techniques used to clean and tokenize the text data before feeding it into the LLM for training or inference.
   - [ ] Embeddings are the ensemble methods used to combine multiple LLMs to improve the overall performance and robustness of the system.
   - [ ] Embeddings are the linguistic rules and grammar patterns extracted from the text data to aid the LLM in understanding and generating language.

4. A company has pre-trained a large language model on a vast corpus of text data. They want to adapt this pre-trained model to perform specific tasks such as sentiment analysis and document summarization. Which of the following best describes the process of fine-tuning?
   - [ ] Fine-tuning involves training the pre-trained language model from scratch.
   - [x] Fine-tuning refers to the process of further training the pre-trained language model on labeled data for the specific tasks.
   - [ ] Fine-tuning is a technique used to preprocess and clean the task-specific data before feeding it into the pre-trained language model.
   - [ ] Fine-tuning is an ensemble method that combines the pre-trained language model with task-specific models to improve the overall performance.

5. A team is tasked with choosing a generative artificial intelligence (AI) model that can recognize and interpret different forms of input data, such as text, images, and audio.Which of the following model architectures is best suited for this task?
   - [ ] Large language model
   - [ ] Diffusion model
   - [x] Multimodal model
   - [ ] Foundation model

---
[⬆️ Go to Context](#context)

# **AWS Infrastructure and Technologies**

AWS rapidly innovates across the AI and ML stack, offering comprehensive capabilities from infrastructure and tools to groundbreaking applications like AI-based coding. Customers value the AWS data-first approach, security, and breadth of enterprise-grade offerings spanning all layers.

---
[⬆️ Go to Context](#context)

## ML frameworks

- The ML frameworks layer plays a crucial role in the development and deployment of machine learning models. At the core of the frameworks layer is Amazon SageMaker AI. SageMaker AI offers the right tools to effectively build, train, and run LLMs and other FMs efficiently and cost effectively. Choose the following tab to learn more about this service.
- **Amazon SageMaker AI:** With SageMaker AI, you can build, train, and deploy ML models for any use case with fully managed infrastructure, tools, and workflows. SageMaker AI removes the heavy lifting from each step of the ML process to make it easier to develop high-quality models. SageMaker AI provides all the components used for ML in a single toolset, so models get to production faster with much less effort and at lower cost.

---
[⬆️ Go to Context](#context)

## AI/ML services

![AWS Services](https://i.imgur.com/8W8chht.png)

AWS provides a robust AI/ML services layer, offering ready-to-use solutions like Amazon Comprehend for natural language processing tasks and Amazon Kendra for intelligent search across organizational data. This layer includes a wide range of services that provide developers with AI/ML capabilities without requiring extensive infrastructure management or specialized expertise.

- **Amazon Comprehend**: Amazon Comprehend uses ML and natural language processing (NLP) to help you uncover the insights and relationships in your unstructured data. This service performs the following functions:
  - Identifies the language of the text
  - Extracts key phrases, places, people, brands, or events
  - Understands how positive or negative the text is
  - Analyzes text using tokenization and parts of speech
  - And automatically organizes a collection of text files by topic
- **Amazon Translate**: Amazon Translate is a neural machine translation service that delivers fast, high-quality, and affordable language translation. Neural machine translation is a form of language translation automation that uses deep learning models to deliver more accurate and more natural-sounding translation than traditional statistical and rule-based translation algorithms. With Amazon Translate, you can localize content such as websites and applications for your diverse users, translate large volumes of text for analysis, and efficiently implement cross-lingual communication between users.
- **Amazon Textract**: Amazon Textract is a service that automatically extracts text and data from scanned documents. Amazon Textract goes beyond optical character recognition (OCR) to also identify the contents of fields in forms and information stored in tables.
- **Amazon Lex**: Amazon Lex is a fully managed AI service to design, build, test, and deploy conversational interfaces into any application using voice and text. Amazon Lex provides the advanced deep learning functionalities of automatic speech recognition (ASR) for converting speech to text, and natural language understanding (NLU) to recognize the intent of the text. This permits you to build applications with highly engaging user experiences and lifelike conversational interactions, and create new categories of products. With Amazon Lex, the same deep learning technologies that power Amazon Alexa are now available to any developer. You can efficiently build sophisticated, natural-language conversational bots and voice-enabled interactive voice response (IVR) systems.
- **Amazon Polly**: Amazon Polly is a service that turns text into lifelike speech. Amazon Polly lets you create applications that talk, so you can build entirely new categories of speech-enabled products. Amazon Polly is an AI service that uses advanced deep learning technologies to synthesize speech that sounds like a human voice. Amazon Polly includes a wide selection of lifelike voices spread across dozens of languages, so you can select the ideal voice and build speech-enabled applications that work in many different countries.
- **Amazon Transcribe**: Amazon Transcribe is an automatic speech recognition (ASR) service for automatically converting speech to text. The service can transcribe audio files stored in common formats, like WAV and MP3, with time stamps for every word so that you can quickly locate the audio in the original source by searching for the text. You can also send a live audio stream to Amazon Transcribe and receive a stream of transcripts in real time. Amazon Transcribe is designed to handle a wide range of speech and acoustic characteristics, including variations in volume, pitch, and speaking rate. Customers can use Amazon Transcribe for a variety of business applications, including the following:
  - Transcription of voice-based customer service calls
  - Generation of subtitles on audio and video content
  - Conducting (text based) content analysis on audio and video content
- **Amazon Rekognition**: Amazon Rekognition facilitates adding image and video analysis to your applications. It uses proven, highly scalable, deep learning technology that requires no ML expertise to use. With Amazon Rekognition, you can identify objects, people, text, scenes, and activities in images and videos, and even detect inappropriate content. Amazon Rekognition also provides highly accurate facial analysis and facial search capabilities. You can use it to detect, analyze, and compare faces for a wide variety of user verification, people counting, and public safety use cases.
- **Amazon Kendra**: Amazon Kendra is an intelligent search service powered by ML. Amazon Kendra reimagines enterprise search for your websites and applications. Your employees and customers can conveniently find the content that they are looking for, even when it’s scattered across multiple locations and content repositories within your organization.
- **Amazon Personalize**: Amazon Personalize is an ML service that developers can use to create individualized recommendations for customers who use their applications. With Amazon Personalize, you provide an activity stream from your application (page views, signups, purchases, and so forth). You also provide an inventory of the items that you want to recommend, such as articles, products, videos, or music. You can choose to provide Amazon Personalize with additional demographic information from your users, such as age or geographic location. Amazon Personalize processes and examines the data, identifies what is meaningful, selects the right algorithms, and trains and optimizes a personalization model that is customized for your data.
- **AWS DeepRacer**: AWS DeepRacer is a 1/18th scale race car that gives you an interesting and fun way to get started with reinforcement learning (RL). RL is an advanced ML technique that takes a very different approach to training models than other ML methods. Its superpower is that it learns very complex behaviors without requiring any labeled training data, and it can make short-term decisions while optimizing for a longer-term goal.

---
[⬆️ Go to Context](#context)

## Generative AI

![Generative AI](https://i.imgur.com/gH2fc1q.png)

The generative AI services layer in the AI and ML stack offers a suite of powerful tools and services specifically designed for generative AI tasks. This layer includes services like SageMaker JumpStart for accelerating model development and deployment. Amazon Bedrock offers a choice of high-performing FMs from leading AI companies through a single API. With these services, developers and organizations can harness the capabilities of generative AI models, unlocking new possibilities for content creation, data synthesis, and interactive AI experiences.

- **Amazon SageMaker JumpStart**: SageMaker JumpStart helps you quickly get started with ML. To facilitate getting started, SageMaker JumpStart provides a set of solutions for the most common use cases, which can be rapidly deployed. The solutions are fully customizable and showcase the use of AWS CloudFormation templates and reference architectures so that you can accelerate your ML journey. SageMaker JumpStart also supports one-click deployment and fine-tuning of more than 150 popular open-source models such as natural language processing, object detection, and image classification models.
- **Amazon Bedrock**: Amazon Bedrock is a fully managed service that makes FMs from Amazon and leading AI startups available through an API. With the Amazon Bedrock serverless experience, you can quickly get started, experiment with FMs, privately customize them with your own data, and seamlessly integrate and deploy FMs into your AWS applications.
- **Amazon Q**: Amazon Q can help you get fast, relevant answers to pressing questions, solve problems, generate content, and take actions using the data and expertise found in your company's information repositories, code, and enterprise systems. When you chat with Amazon Q, it provides immediate, relevant information and advice to help streamline tasks, speed decision-making, and help spark creativity and innovation.
- **Amazon Q Developer**: Designed to improve developer productivity, Amazon Q Developer provides ML–powered code recommendations to accelerate development of C#, Java, JavaScript, Python, and TypeScript applications. The service integrates with multiple integrated development environments (IDEs) and helps developers write code faster by generating entire functions and logical blocks of code—often consisting of more than 10–15 lines of code.

---
[⬆️ Go to Context](#context)

# **QnA on AWS Services**

1. A company has a large collection of customer support emails and chat transcripts. They want to analyze the sentiment expressed in these messages and identify common issues or topics discussed by their customers.Which AWS service would be most appropriate for this task?
   - [ ] Amazon Transcribe
   - [ ] Amazon Kendra
   - [ ] Amazon Polly
   - [x] Amazon Comprehend

2. A retail company has accumulated a large volume of customer transaction data, including purchase history, product preferences, and demographic information. The company wants to use this data to build machine learning models that can provide personalized product recommendations to customers and improve their overall shopping experience. Which AWS service would be most suitable for the retail company to build, train, and deploy machine learning models for personalized product recommendations?
   - [x] Amazon SageMaker AI
   - [ ] Amazon Bedrock
   - [ ] Amazon Lex
   - [ ] Amazon Q Developer

---
[⬆️ Go to Context](#context)