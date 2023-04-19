**Independent and Identically Distributed (IID)**

In federated learning, Independent and Identically Distributed (IID) is a property that refers to the data distribution of the participating clients.

**Independent** means that the data from each client is unrelated to the data from other clients. This means that each client has its own unique set of data, and the data from one client does not depend on the data from other clients.

**Identically Distributed** means that the data from each client is drawn from the same probability distribution. This means that each client's data is similar to the data of other clients, in terms of the features and labels they contain.

Technical definition of an IID statistics is:


Having IID data is important in federated learning because it enables the central server to train a global model that can generalize well to new data. When the data from all clients is IID, the central server can combine the data from different clients to create a more diverse and representative dataset, which can improve the overall performance of the model. However, when the data is not IID, such as when some clients have more data than others or when the data from different clients has different distributions, it can be more challenging to train a model that performs well on all clients.
To assume we have MNIST dataset D with length 60K (60,000 images), and 10 (num_client=10) clients will participate in the training process. According to the IID principle, we will distribute D to all clients (10 clients) equally. The figure follows the distribution process based on IID settings. 
 
![image](https://user-images.githubusercontent.com/23058510/230216323-e749f227-a1a5-4ae1-b4df-9ab7f72a055c.png)

Where each group is independent of other groups, and each all group has the same size and the same data structure
