---
mindmap-plugin: basic
tags:
  - CompSci/AI/ML/model/classification
  - CompSci/AI/ML/MLFlow
---
# MLflow models
### Description:
- Standard format for packaging machine learning models that can be used in a variety of downstream tools
- 
### Storage format:
- [[MLFlow flavor]]
	- All of the flavors that a particular model supports are defined in its `MLmodel` file in YAML format
- If you wish to serve a model from inside a Docker container  (or to query it from another machine)
	- you need to change the network address to `0.0.0.0` using the `-h` argument.
	  ```bash
	  mlflow models serve -h 0.0.0.0 -m my_model
	  ```
-  
### Model signature and input examples:
- [[Model inference param]]:
	- description of params used for model inference
- [[Model signature]]
- 
