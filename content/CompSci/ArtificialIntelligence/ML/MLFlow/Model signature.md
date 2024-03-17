---
mindmap-plugin: basic
tags:
  - CompSci/AI/ML/model/classification
  - CompSci/AI/ML/MLFlow
---
# Model signature
### Description:
- Description of a model’s inputs, outputs and parameters.
- Example:
	- 
	  ```yaml
	  signature:
	  inputs: '[{"name": "text", "type": "string"}]'
    outputs: '[{"name": "output", "type": "string"}]'
    params: '[{"name": "temperature", "type": "float", "default": 0.5, "shape": null},
              {"name": "top_k", "type": "integer", "default": 1, "shape": null},
              {"name": "suppress_tokens", "type": "integer", "default": [101, 102], "shape": [-1]}]'
		```
### Column-based Signature:

### Tensor-based Signature :

### Signature with params :