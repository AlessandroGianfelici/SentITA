# Sentita
Sentiment polarity classification in Italian

Currently Sentita is an alpha version

How to install Sentita:
1. Dowload Sentita from this [link][https://drive.google.com/file/d/1s1BW3T_BysAhVZPai-3AUXpb68aYjQTS/view?usp=sharing]
2. Unzip the archive
3. cd into the unzipped folder from the console
4. type in the console "pip install ." to install the package locally


How to use Sentita:
1. Import the function to calculate the polarity scores with the following code:
	from sentita import calculate_polarity
	
2. Define your sentences as a list. e.g.:
	sentences = ["il divano era molto comodo",
				 "il cibo era davvero buono",
				 "il posto era davvero accogliente e i camerieri simpatici, consigliato!"]

3. Estimate the sentence polarity by running:
	results, polarities = calculate_polarity(sentences)
	
	"results" is a list of texts with the sentence, the positive polarity score and the negative polarity scores.
	"polarities" is a list of lists with the positive and negative polarity score for each sentence, e.g.:
		polarities[0][0] contains the positive polarity score of the 1st sentence
		polarities[2][0] contains the positive polarity score of the 3rd sentence
		polarities[2][1] contains the negative polarity score of the 3rd sentence
