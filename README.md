# 	• Low Bias >> Less Assumptions >> Non Parametric functions >> Complex Model>> High Variance >> Overfitting
	• High Bias >> More Assumptions >> Parametric Functions >> Simple Model >> Low Variance >> Underfitting
	• Bias vs. Variance
		○ Bias measures how inaccurate the model prediction is in comparison with the true output. 
			§ It is due to erroneous assumptions made in the machine learning process to simplify the model and make the target function easier to learn. 
			§ High model complexity tends to have a low bias.
			§ Bias: Error that results from inaccurate assumptions in model training (that are made to simplify the training process)
		

		○ Variance measures how much the target function will change if different training data is used. 
			§ Variance can be caused by modeling the random noise in the training data.
			§  High model complexity tends to have a high variance.
			§ Varience: Error that occurs when the model is too sensitive to the training data (thus giving different estimates when given new training data)
			
		○ As a general trend, parametric and linear algorithms often have high bias and low variance, whereas non-parametric and non-linear algorithms often have low bias and high variance
		
	• Overfitting vs. Underfitting
		○ Overfitting refers to the situation in which models fit the training data very well, but fail to generalize to new data.
			§ In statistics, Variance informally means how far your data is spread out. Overfitting is you memorise 10 qns for your exam and on the next day exam, only one question has been asked in the question paper from that 10 you read. Now you will answer that one qn correctly just like in the book, but you have no idea what the remaining questions are(Question are HIGHLY VARIED from what you read). In overfitting, model will memorise the entire train data such that it will give high accuracy on train but will suck in test. Hope its helps
		
		○ Underfitting refers to the situation in which models neither fit the training data nor generalize to new data.
			§ Underfitting is called "Simplifying assumption" (Model is HIGHLY BIASED towards its assumption). your model will think linear hyperplane is good enough to classify your data which may not be true. consider you are shown a picture of cat 1000 times, Now you are blindfolded, No matter Whatever you are shown the 1001th time, probability that you will say cat is very high(You are HIGHLY BIASED that the next picture is also gonna be a cat). Its because you believe its gonna be a cat anyway. Here you are simplifying assumptions
			
				
	

	• Prediction Error
		○ prediction error = Bias error + variance + error + irreducible error
	
		○ Low bias means fewer assumptions about the target function.
			§ Some examples of algorithms with low bias are KNN and decision trees. 
			§ Having fewer assumptions can help generalize relevant relations between features and target outputs. 
		○ high bias means more assumptions about the target function.
			§ Linear regression would be a good example (e.g., it assumes a linear relationship). 
			§ Having more assumptions can potentially miss important relations between features and outputs and cause underfitting.
		○ Low variance indicates changes in training data would result in similar target functions. 
			§ For example, linear regression usually has a low variance.
		○  High variance indicates changes in training data would result in very different target functions.
			§ For example, support vector machines usually have a high variance. 
			§ High variance suggests that the algorithm learns the random noise instead of the output and causes overfitting.
	• Generally, increasing model complexity 
		○ would decrease bias error since the model has more capacity to learn from the training data. 
		○ But the variance error would increase if the model complexity increases, as the model may begin to learn from noise in the training data.
	• The goal of training machine learning models is to achieve 
		○ low bias and low variance. 
		○ The optimal model complexity is where bias error crosses with variance error.
		
		

	
	
		
				□ R: close to 1 means more accurate
		
	• LIMITING OVERFITTING
		○ k-fold cross-validation: it split the initial training data into k subsets and train the model k times. In each training, it uses one subset as the testing data and the rest as training data.
		○ hold back a validation dataset from the initial training data to estimatete how well the model generalizes on new data.
		○ simplify the model. For example, using fewer layers or less neurons to make the neural network smaller.
		○ use more data.
		○ reduce dimensionality in training data such as PCA: it projects training data into a smaller dimension to decrease the model complexity.
			§ PCA reduces the training data dimensionality and can reduce model complexity
		○ Stop the training early when the performance on the testing dataset has not improved after a number of training iterations.
			§ You can limit overfitting by stopping the training when performance on the test data does not improve.


	

		
	





	• QUIZZES








