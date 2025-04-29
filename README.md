# foundations-of-natural-language-processing-coursework-2-solved
**TO GET THIS SOLUTION VISIT:** [Foundations of Natural Language Processing Coursework 2 Solved](https://www.ankitcodinghub.com/product/coursework-2-foundations-of-natural-language-processing-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;116097&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;Foundations of Natural Language Processing Coursework 2 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
1 Introduction

This coursework consists of three parts in which you demonstrate your understanding of fundamental concepts and methods of Natural Language Processing. The coursework contains open questions and programming tasks with Python using NLTK. This coursework is worth 12.5% of your final mark for the course. It is marked out of 100.

The files with the template code you need are on the LEARN page for the assignment (click on “Assessment” on the LHS menu, then “Coursework 2 – Hidden Markov Models”). You will download a file called assignment2.tar.gz which can be unpacked using the following command to a shell prompt:

tar -xf assignment2.tar.gz

This will create a directory assignment2 which contains additional Python modules used in this coursework, together with a file named template.py, which you must use as a starting point when attempting the questions for this assignment.

There is an interim checker that runs some automatic tests that you can use to get partial feedback on your solution: https://homepages.inf.ed.ac.uk/cgi/ht/fnlp/interim2 22.py

Submission

Before submitting your assignment:

• Ensure that your code works on DICE. Your modified template.py should fully execute using python3 with or without the answer flag.

• Any character limits to open questions will be strictly enforced. Answers will be passed through an automatic filter that only keeps the first N characters, where N is the character limit given in a question.

When you are ready to submit, rename your modified template.py with your matriculation number: e.g., s1234567.py.

//web.inf.ed.ac.uk/infweb/student-services/ito/admin/coursework-projects/late-co ursework-extension-requests. Do not email any course staff directly about extension requests; you must follow the instructions on the web page.

Furthermore, you are required to take reasonable measures to protect your assessed work from unauthorised access. For example, if you put any such work on a public repository (e.g., GitHub), then you must set access permissions appropriately (for this coursework, that means only you should be able to access it).

In this part of the assignment you have to train a Hidden Markov Model (HMM) for part-of-speech (POS) tagging. Look at the solutions from Lab 3, Exercise 3 and Exercise 4 as a reminder for what you have to compute.

You will need to create and train two models—an Emission Model and a Transition Model as described in lectures.

Use labelled sentences from the ‘news’ part of the Brown corpus. These are annotated with parts of speech, which you will convert into the Universal POS tagset (NLTK uses the smaller version of this set defined by Petrov et al.1). Having a smaller number of labels (states) will make Viterbi decoding faster.

We will use the last 500 sentences from the corpus as the test set and the rest for training. This split corresponds roughly to a 90/10% division.

Estimate the Emission model: Fill in the emission model method of the HMM class. Use a

ConditionalProbDist with a LidstoneProbDist estimator.

Review the help text for the ConditionalProbDist class. Note that the probdist factory argument to its init method can be a function that takes a frequency distribution and returns a smoothed probability distribution based on it (i.e. an estimator).

Review the help text for the LidstoneProbDist class and look particularly at the arguments to the init method. You should implement a function to pass to ConditionalProbDist which creates and returns a LidstoneProbDist based on the input frequency distribution, using +0.001

1 https://github.com/slavpetrov/universal-pos-tags

for smoothing and adding an extra bin (which will be used for all ”unknown” tokens, i.e. tokens not seen in the training set).

Convert all the observations (words) to lowercase.

Store the result in the variable self.emission PD. Save the states (POS tags) that were seen in training in the variable self.states. Both these variables will be used by the Viterbi algorithm in Section B.

Define an access function elprob for the emission model by filling in the function template provided.

Estimate the Transition model. Fill in the transition model method of the HMM class. Use a ConditionalProbDist with a LidstoneProbDist estimator using the same approach as in Question 1 but without the extra ‘bin’ (because we assume all POS tags are seen in training).

When using the training data for this step, add a start token (&lt;s&gt;,&lt;s&gt;) and an end token (&lt;/s&gt;,&lt;/s&gt;) to each sentence, so that the resulting matrix has useful transition probabilities for transitions from &lt;s&gt; to the real POS tags and from the real POS tags to &lt;/s&gt;. For example, for this sentence from the training data:

[( ‘ Ask ’ , ‘VERB’) , ( ‘ jail ’ , ‘NOUN’) , ( ‘ deputies ’ , ‘NOUN’ ) ]

you would use this as part of creating the transition model:

[(&lt;s&gt;,&lt;s &gt;) ,( ‘Ask ’ , ‘VERB’) , ( ‘ jail ’ , ‘NOUN’) , ( ‘ deputies ’ , ‘NOUN’) ,

(&lt;/s&gt;,&lt;/s &gt;)]

Store the model in the variable self.transition PD. This variable will be used by the Viterbi algorithm in Section B.

Define an access function tlprob for the transition model by filling in the function template provided.

In this part of the assignment you have to implement the Viterbi algorithm. The pseudo-code of the algorithm can be found in the Jurafsky &amp; Martin 3rd edition book in Appendix A Figure A.9 in section A.4: use it as a guide for your implementation.

However you will need to add to J&amp;M’s algorithm code to make use of the transition probabilities to &lt;/s&gt; which are also now in the a matrix.

In the pseudo-code the b probabilities correspond to the emission model implemented in part A, question 1 and the a probabilities correspond to the transition model implemented in part A, question 2. You should use costs (negative log probabilities). Therefore instead of multiplication of probabilities (as in the pseudo-code) you will do addition of costs, and instead of max and argmax you will use min and argmin.

Note that per the instructions for Question 2 above, you will not need a separate π tabulation for the initialisation step, because we’ve included start state probabilities in the a matrix as transitions from &lt;s&gt; and you can use that.

Fill in the access functions get viterbi value and get backpointer value so that your Viterbi implementation can be queried without the caller needing to know how you implemented your data structures.

The argument observations is a list of words representing the sentence to be tagged. Remember to use costs. The nested loops of the recursion step have been provided in the template. Fill in the code inside the loops for the recursion step. Describe your implementation with comments.

Finally, fill in tag sentence, which takes a sentence as input, initialises the HMM, runs the Viterbi algorithm and returns the tags. Don’t forget to lower case the tokens and don’t clear the memory of the viterbi and backpointer data structures because the automarking procedure will call get viterbi value and get backpointer value.

Modify compute acc so it prints the first 10 tagged test sentences which did not match up with their ‘correct’ versions (taken from the tagged test data as supplied). Inspect these. Why do you think these have been tagged differently by the model? Pick one sentence and give a short answer discussing this. Be sure to consider the possibility that in some cases it’s the corpus tag which is

‘incorrect’.

Write down your answer in the answer question4b function, returning the sentence as tagged by your model, the official ’correct’ version and your commentary.

Copy-paste the ”correctly” tagged sentence and the output of your model them from your output into answer question4b.

There is a 280 character limit on the answer to this question.

Require: Labeled data L, unlabeled data U, number of iterations k.

1: procedure Semi-supervised Hard EM(L,U,k)

2: T0 ← train HMM on labeled data L

3: for i ∈ ⟨0,…,k − 1⟩ do

4: Let Pi+1 be U labelled according to Ti

5: Ti+1 ← HMM trained on L and Pi+1

Below is a sentence from the corpus with the gold POS tags it was annotated with, the most likely tags according to the model which was trained on the 20 sentences (T0) and the most likely tags according to a the model trained with hard EM for 3 iterations (Tk):

Sentence In fact he seemed delighted to get rid of them .

Gold POS ADP NOUN PRON VERB VERB PRT VERB ADJ ADP PRON .

T0 PRON VERB NUM ADP ADJ PRT VERB NUM ADP PRON .

Tk PRON VERB PRON VERB ADJ PRT VERB NUM ADP NOUN .

1. T0 erroneously tagged “he” as “NUM” and Tk correctly identifies it as “PRON”. Speculate why additional unlabeled data might have helped in that case. Refer to the training data (inspect the 20 sentences!).

2. Where does Tk mislabel a word but T0 is correct? Why do you think did hard EM hurt in that case?

Write down your answer in the answer question5b function. There is a 500 character limit for this question.

Suppose you have a hand-crafted probabilistic context-free grammar and lexicon that has 100% coverage on constructions but less than 100% lexical coverage. How could you use a pre-trained POS tagger to ensure that the grammar produces a parse for any well-formed sentence, even when the grammar doesn’t recognise the words within that sentence?

Will your approach always do as well or better than the original parser on its own? Why or why not?

Write down your answer in the answer question6 function. There is a 500 character limit on the answer to this question.

Why else, besides the speedup already mentioned above, do you think we converted the original Brown Corpus tagset to the Universal tagset? What do you predict would happen if we hadn’t done that? Why?

Write down your answer in the answer question7 function. There is a 500 character limit on the answer to this question.
