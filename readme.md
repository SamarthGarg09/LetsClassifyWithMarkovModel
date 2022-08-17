# Poem Classification and Generation 

* ### Build markov model from scratch and along with conditional probability used it to classify between authors and used it for generating poem.

> Markov rule - The current state depends only on its previous state

> $ P(x1, x2, x3) = P(x1)*P(x2/x1)*p(x3/x2)$ 
* Notice that conditional probabilites just depends on one previous state this is the assumption which we'll be carrying to build this model.

### Datset link : 
* [Alan's poem](https://raw.githubusercontent.com/lazyprogrammer/machine_learning_examples/master/hmm_class/edgar_allan_poe.txt
)
* [Robert's poem](https://raw.githubusercontent.com/lazyprogrammer/machine_learning_examples/master/hmm_class/robert_frost.txt
)

### Binary classification task
* class 0: Edger Alan Poe
* class 1: Robert Frost

### Confusion metrics
<img src="confusion-metrics.png" alt="poem_classification" style="width:70%;">

### Test and Train accuracy
* Train Accuracy : 0.897
* Test Accuracy : 0.75

### To select the next most apt word while generating poem we used normal sampling technique to avoid repeatitions.

### For live inference one can run the model on gradio too!
