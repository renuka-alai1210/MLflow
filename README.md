# MLflow
An open source platform for the machine learning lifecycle.
MLflow is an open source platform to manage the ML lifecycle, including experimentation, reproducibility, deployment, and a central model registry. MLflow currently offers four components:


![1_zrGyk6kdaiGUXxY8MXOQ9A](https://user-images.githubusercontent.com/55275843/178004915-06695ab2-3cf4-425a-a551-51bb681d185c.png)

# MLflow Tracking
MLflow Tracking is an API and UI for logging parameters, code versions, metrics, and artifacts when running your machine learning code and for later visualizing the results. You can use MLflow Tracking in any environment (for example, a standalone script or a notebook) to log results to local files or to a server, then compare multiple runs. Teams can also use it to compare results from different users
![Screenshot from 2022-06-14 10-30-22](https://user-images.githubusercontent.com/55275843/178005236-5f40992f-aeba-4959-bc8c-099c072f2a4d.png)

# MLflow Projects
MLflow Projects are a standard format for packaging reusable data science code. Each project is simply a directory with code or a Git repository, and uses a descriptor file or simply convention to specify its dependencies and how to run the code. For example, projects can contain a conda.yaml file for specifying a Python Conda environment. When you use the MLflow Tracking API in a Project, MLflow automatically remembers the project version (for example, Git commit) and any parameters. You can easily run existing MLflow Projects from GitHub or your own Git repository, and chain them into multi-step workflows.
![Screenshot from 2022-06-14 10-31-00](https://user-images.githubusercontent.com/55275843/178005464-2b31f870-8076-473d-9101-17556480f109.png)

# MLflow Models
MLflow Models offer a convention for packaging machine learning models in multiple flavors, and a variety of tools to help you deploy them. Each Model is saved as a directory containing arbitrary files and a descriptor file that lists several flavors the model can be used in. For example, a TensorFlow model can be loaded as a TensorFlow DAG, or as a Python function to apply to input data. MLflow provides tools to deploy many common model types to diverse platforms: for example, any model supporting the Python function flavor can be deployed to a Docker-based REST server, to cloud platforms such as Azure ML and AWS SageMaker, and as a user-defined function in Apache Spark for batch and streaming inference. If you output MLflow Models using the Tracking API, MLflow also automatically remembers which Project and run they came from.
![Screenshot from 2022-06-14 10-31-41](https://user-images.githubusercontent.com/55275843/178005637-56004100-538a-4b33-900e-39c463f27d01.png)

# Model Registry
MLflow Registry offers a centralized model store, set of APIs, and UI, to collaboratively manage the full lifecycle of an MLflow Model. It provides model lineage (which MLflow experiment and run produced the model), model versioning, stage transitions (for example from staging to production or archiving), and annotations.
![model-registry-new](https://user-images.githubusercontent.com/55275843/178006119-ffb9a9be-272c-425f-ab09-edef05079979.png)
