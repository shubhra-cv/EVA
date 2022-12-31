The heart of the solution is the network class.
Here is the summary of same: <br>
The code is defining a class called Network, which is a neural network module. The __init__() method initializes the network with two convolutional layers (conv1 and conv2), two fully connected layers (fc1 and fc2), one fully-connected layer (fc3) for combining the inputs from conv1 and conv2, and two output layers (out_i and out_rn). The forward() method defines the forward pass of the network, taking in an input (t) and a one-hot encoded random number (rand_num_ohe) as inputs. The input is passed through the convolutional layers, followed by the fully-connected layers, and finally the output layers. The output layers return two values, x_image and x_sum.

Training Logs:
total_loss = 0.8(loss1(Image)) + 0.2(loss2(Sum)) <br> 
<br>
epoch 0 total_correct_image: 56770 total_correct_sum: 38823 loss: tensor(0.1702, device='cuda:0', grad_fn=<AddBackward0>)<br>
epoch 1 total_correct_image: 58472 total_correct_sum: 57245 loss: tensor(0.5585, device='cuda:0', grad_fn=<AddBackward0>)<br>
epoch 2 total_correct_image: 58681 total_correct_sum: 57908 loss: tensor(0.9654, device='cuda:0', grad_fn=<AddBackward0>)<br>
epoch 3 total_correct_image: 58864 total_correct_sum: 58040 loss: tensor(0.0095, device='cuda:0', grad_fn=<AddBackward0>)<br>
epoch 4 total_correct_image: 58873 total_correct_sum: 58088 loss: tensor(0.6852, device='cuda:0', grad_fn=<AddBackward0>)<br>
epoch 5 total_correct_image: 58966 total_correct_sum: 58253 loss: tensor(0.1924, device='cuda:0', grad_fn=<AddBackward0>)<br>
epoch 6 total_correct_image: 58947 total_correct_sum: 58227 loss: tensor(0.4302, device='cuda:0', grad_fn=<AddBackward0>)<br>
epoch 7 total_correct_image: 59044 total_correct_sum: 58374 loss: tensor(0.1567, device='cuda:0', grad_fn=<AddBackward0>)<br>
epoch 8 total_correct_image: 59038 total_correct_sum: 58406 loss: tensor(0.1140, device='cuda:0', grad_fn=<AddBackward0>)<br>
epoch 9 total_correct_image: 59093 total_correct_sum: 58476 loss: tensor(0.1662, device='cuda:0', grad_fn=<AddBackward0>)<br>