
# Video Summarization with ResNeXt and LSTM 
Ever wished you could get a quick highlight reel of your favorite TV show or an important lecture? Look no further! This project is an implementation of a video summarization model that harnesses the power of ResNeXt for feature extraction and an LSTM network for sequence modeling. Our model is designed to predict the importance scores of video frames, which can then be used to generate a concise and engaging summary of any video. This project was created in Spring '22 for ACM AI at UC San Diego.

### Overview
In this repository, you'll find the code for training and evaluating our video summarization model. By leveraging a pretrained ResNeXt network to extract features from video frames and an LSTM network to predict the importance scores of these frames, our model captures the essence of the video content. The importance scores are then used to select the most crucial frames, creating a summary that's both informative and entertaining.

### Model Architecture

#### Encoder
Our encoder is the heavyweight of feature extraction, using a pretrained ResNeXt model. This powerful network dives into each video frame and extracts a feature vector, essentially capturing the frame's most significant details and nuances.

#### RNN Model
The RNN model, powered by an LSTM network, is the brain behind predicting the importance scores of the frames based on the features extracted by ResNeXt. Think of it as a meticulous editor who knows exactly which scenes make the cut. The network consists of several LSTM layers followed by fully connected layers, ensuring it captures the sequential nature of the video.

### Training
Training our model is like a rigorous workout session. The training loop iterates through the dataset, passing batches of frames through the encoder and RNN model. It computes the loss and gradients to update the model parameters, ensuring our model gets smarter with each iteration.

### Evaluation
Evaluating the model is akin to a performance review. The evaluation loop iterates through the validation dataset, computing the loss and predictions to assess how well our model is doing. It helps us fine-tune the model, making sure it picks out the best highlights every time.
