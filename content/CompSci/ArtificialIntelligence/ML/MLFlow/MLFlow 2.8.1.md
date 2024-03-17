---
mindmap-plugin: basic
tags:
  - CompSci/AI/ML/MLFlow
  - CompSci/tool/pip
aliases:
  - mlflow
---
# MLFlow
### Description:
- Managing machine learning life cycle
### Core Components of MLflow
- [[MLflow tracking]]
- [[MLflow model registry]]
- [[MLflow models]]
- [[MLflow evaluate]]: 
	- Designed for in-depth model analysis, this set of tools facilitates objective model comparison, be it traditional ML algorithms or cutting-edge LLMs.
    
- [Prompt Engineering UI](https://mlflow.org/docs/latest/llms/prompt-engineering/index.html#prompt-engineering): 
	- A dedicated environment for prompt engineering, this UI-centric component provides a space for prompt experimentation, refinement, evaluation, testing, and deployment.
	- In experimental
- [Recipes](https://mlflow.org/docs/latest/recipes.html#recipes): 
	- Serving as a guide for structuring ML projects, Recipes, while offering recommendations, are focused on ensuring functional end results optimized for real-world deployment scenarios.
- [Projects](https://mlflow.org/docs/latest/projects.html#projects): 
	- MLflow Projects standardize the packaging of ML code, workflows, and artifacts, akin to an executable. 
	- Each project, be it a directory with code or a Git repository, employs a descriptor or convention to define its dependencies and execution method.
- [AI Gateway](https://mlflow.org/docs/latest/llms/gateway/index.html#gateway): experimental
	- This server, equipped with a set of standardized APIs, streamlines access to both SaaS and OSS LLM models. It serves as a unified interface, bolstering security through authenticated access, and offers a common set of APIs for prominent LLMs.
### [[mlflow Python]]
### [[mlflow CLI]]