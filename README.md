# Register And Deploy Trained ML Models on Amazon SageMaker AI using boto3

This repo is built for [Amazon SageMaker AI](https://aws.amazon.com/sagemaker/ai/) users that would like to deplopy their existing trained machine learning models (that were trained outside the AWS Cloud) for inference using our lower level SDK, [boto3](https://boto3.amazonaws.com/v1/documentation/api/latest/index.html). It contains a Jupyter Notebook demonstrating the steps you'd have to take to upload, configure and deploy your model to a SageMaker Inference Endpoint. The notebook configures and deploys a pre-trained ResNet-50 model that comes with PyTorch as an example, but its steps are incredibly similar to what migrating other machine learning models would be. There are annotations of how you can fit the notebook's boto3 invocations and code for your own model, with flexibility depending on your model's machine learning framework (eg. PyTorch, Tesnorflow, etc), hardware (eg. x86, ARM, cuda) and more.

## Overview

The notebook covers the following steps:

1. Generate an inference script that will interfact with your model so it can run on SageMaker AI managed infrastructure.
2. Prepare the model as a Model Artifact
3. Register the model in the SageMaker AI Model Registry
4. Create a SageMaker AI Endpoint Configuration
5. Deploy the model to a SageMaker AI Inference Endpoint using the created resources
6. Invoke the deployed model for inference

## Security

See [CONTRIBUTING](CONTRIBUTING.md#security-issue-notifications) for more information.

## License

This library is licensed under the MIT-0 License. See the LICENSE file.

