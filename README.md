# Installation
Clone this repository and install the dependencies:
```bash
git clone https://github.com/liangchingyun/A-Convolution-Module-For-Variable-Input-Channels.git
```
```bash
cd A-Convolution-Module-For-Variable-Input-Channels
```
```bash
pip install -r requirements.txt
```

# Running Jupyter Notebook
Make sure you have Jupyter Notebook installed. If not, you can install it using the following command:
```bash
pip install jupyter
```
Navigate to the cloned repository directory and open the main.ipynb file.

# Modifying Training Parameters

You can modify the training parameters below to customize your training process. Here's a brief description of each parameter:

- `batch_size`: The batch size used for training.
- `test_batch_size`: The batch size used for testing.
- `epochs`: The number of epochs to train the model.
- `learning_rate`: The learning rate used by the optimizer.
- `momentum`: The momentum used by the optimizer.
- `weight_decay`: The weight decay (L2 penalty) applied to the model parameters.

To change these parameters, simply update their values in the code cell below.
```
parser.add_argument('--batch-size', type=int, default=256)
parser.add_argument('--test-batch-size', type=int, default=20)
parser.add_argument('--epochs', type=int, default=100)
parser.add_argument('--lr', type=float, default=0.1, )
parser.add_argument('--momentum', type=float, default=0.9)
parser.add_argument('--weight-decay', type=float, default=1e-4)
parser.add_argument('--net-name', default='resnet18')
parser.add_argument('--channel', default='RG')
```