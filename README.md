# anomalyDetection
Algorithm for Training
Step 1: Input the video by mounting the respective dataset from the drive.
Step 2: Import all the necessary libraries.
Step 3: Define the required functions such as create_dir(), remove_old_images(), store(), load_model() and mean_squared_loss().
Step 4:  After defining the source path for the training videos, separate each video into frames using ffmpeg which is a command-line tool that converts video formats into frames.
Step 5: Convert each frame to a gray image and use Gaussian Blur to remove noise from the frame to increase the efficiency of our model.
 Step 6: Display the subplots using the imshow() function from OpenCV.
Step 7: Convert them to .npy format 
Step 8: We then split the data into training and validation splits.
Step 9:  Give the training split videos as an input to our LSTM model to train the model with the most suitable hyper-parameters which
●	Develops a model in which the loss is minimized and accuracy is increased.
●	Loss is exactly the difference between the mean and hypothesis value in a Gaussian analysis.
Step 10: Next, the graphs are plotted between Training vs Validation accuracy and Training vs Validation loss.
Step 11: The model is set ready for testing.
Algorithm for Testing
Step 1: Train the model using the validation split.
Step 2: Separate each video into frames much similar to training.
Step 3: Convert each frame to a gray image and use Gaussian Blur to apply denoising to the frame.
Step 4: Convert them to .npy format.
Step 5: Give it as an input to the trained LSTM model, so that a value of the loss for each frame is fetched.
Step 6: Even if the value of loss of one frame is higher than the threshold then that video is labelled as an anomaly.
Step 7: Else the video is labelled a normal video.
Step 8: Then the subplots are plotted which is labelled whether the video is either anomaly or normal.
Step 9: Finally, a random video is tested and the output is respectively shown.

