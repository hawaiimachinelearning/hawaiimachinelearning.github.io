---
layout: default
---
The first Hawaii Machine Learning Kaggle Competition has been completed! Thanks to everyone that participated! See the links for information on the competition, tutorials, and results! 


## Hawaii Machine Learning Challenge - Tutorial 1

**Exploratory Data Analysis (EDA) and Feature Engineering** – EDA is one of the first
steps in a machine learning pipeline. It is where analysts gain intuition about the dataset.
Feature engineering is the process in which raw data is transformed into informative
representations (known as features). Feature engineering provides an opportunity for analysts
to impart their intuition and domain expertise into the machine learning pipeline.

In this tutorial we will perform EDA and feature engineering using the competition data.  R and Python code will be provided.


_If you are looking to participate in the competition please use the following [link](https://www.kaggle.com/t/85d5f53d2a0244a7bf1283be7381849d)._



{% assign posts_count = paginator.posts | size %}

<div class="home">
  {% if posts_count > 0 %}
    <div class="posts">
      {% for post in paginator.posts %}
        <div class="post py3">
          <p class="post-meta">{{ post.date | date: site.date_format }}</p>
          <a href="{{ post.url | prepend: site.baseurl }}" class="post-link"><h3 class="h1 post-title">{{ post.title }}</h3></a>
          <span class="post-summary">
            {% if post.summary %}
              {{ post.summary }}
            {% else %}
              {{ post.excerpt }}
            {% endif %}
          </span>
        </div>
      {% endfor %}
    </div>

    {% include pagination.html %}
  {% else %}
    <h1 class='center'>{{ site.text.index.coming_soon }}</h1>
  {% endif %}
</div>
