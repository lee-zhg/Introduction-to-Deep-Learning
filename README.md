# Data & AI Workshop - Deep Learning

## Objective

This workshop will walk you through model development stages of the Data Science / ML workflow. We will be exploring different ways to build deep learning models and deploying those models. By the end of these labs/tutorials, you should understand:

- Developing Deep Learning Models in Watson Studio
- The process of implementing hyper-parameter optimization of Deep Learning models

The instructions were adapted from https://github.com/jrtorres/dsai-workshop-deeplearning.


### Tools Used

- Watson Studio [(docs)](https://dataplatform.cloud.ibm.com/docs/content/wsj/getting-started/welcome-main.html?audience=wdp)
- Watson Machine Learning [(docs)](https://developer.ibm.com/clouddataservices/docs/ibm-watson-machine-learning/get-started/)
- [Jupyter Notebooks](http://jupyter.org/)


## Requirements

- [IBM Cloud Account](https://cloud.ibm.com)


### Prerequisites

1. Store this repository on your local computer.

   If you have GIT on your machine, clone this repository locally. Open a terminal and run:

   ```
   $ git clone https://github.com/lee-zhg/Introduction-to-Deep-Learning.git
   ```

   If you do NOT have GIT on your machine, you can just download the repository as a ZIP file. In the browser window, select :

    ![Download Repo](docs/images/ss0.png)

1. Ensure you have access to a Waston Studio Instance. If you need to provision an instance, see the instructions in the [Setup Watson Studio doc](SetupWatsonStudio.md)

1.  Upload data to IBM Cloud Object Storage

    To upload data,

    - Login to https://cloud.ibm.com
    - If you already have a `Storage` section under the `Resource Summary`,
        - Expand `Storage` under the `Resource Summary`. Create a new instance if you don't have any.
        - Select your storage instance.
    - If you don't have a `Storage` section under the `Resource Summary`,
        - Select `Catalog`.
        - Select `Storage` on the left and then `Object Storage` on the right.
        - Assign a `Service name` and take the default for the rest fields.
        - `Create`.
    - Click `Create bucket` button.
    - Select `Customize bucket` tile.
    - Name your bucket, for example `mybucket-xyz`. The name must be unique
    - Select `Cross Region` for `Resilency`.
    - Select `us-geo` for `Location`.
    - Accept all other defaults.
    - Click the `Create bucket` button.
    - Click `Upload` and then select `File`.
    - Select `Standard Upload`.
    - Click `Select files`.
    - Navigate to the folder where you download and store this repository.
    - Move to the `data` subfolder.
    - Select file
        - training_data.pickle
        - test_data.pickle
        - validation_data.pickle
    - Click `Upload`.


### Lab 1 - Building A Deep Learning Model Using Code

This lab begins by introducing you to Deep Learning through a Jupyter notebook environment using the Keras framework. You will be building a Deep Learning model in a Jupyter Notebook using Keras on timeseries data. Then deploy and consume the trained Deep Learning model as an API on the Watson Machine Learning Service.

[Follow the lab instructions here](https://github.com/lee-zhg/timeseries-rnn-lab-part1)


### Lab 2 - Building A Deep Learning Model Using Visual Assembly

Now that we've built deep learning models and run some experiments, lets look at a different approach to building these DL models. In this case we will explore how to build models using a visual assembly tool called Neural Network Modeler.

[Follow the instructions here](NNModeler-ICFHR.md)


## General Links

- [IBM Developer](https://developer.ibm.com)
- [Watson Studio](https://dataplatform.ibm.com/)
- [Watson Studio Overview](https://dataplatform.cloud.ibm.com/docs/content/wsj/getting-started/overview-ws.html?audience=wdp&context=wdp&linkInPage=true)
- [Watson Machine Learning Python SDK](https://wml-api-pyclient.mybluemix.net/)
- [Watson Studio Video Learning Center](https://www.youtube.com/playlist?list=PLzpeuWUENMK3u3j_hffhNZX3-Jkht3N6V)
- [Data Science Code Patterns](https://developer.ibm.com/code/technologies/data-science/)
