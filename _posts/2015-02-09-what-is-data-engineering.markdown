---
layout: post
title:  "What is Data Engineering?"
date:   2015-02-09
---

Lately, I have been speaking with several candidates for a data engineering role at LearnVest. The question that I find myself frequently answering is, “what does a data engineer do?” This question has been posed by many in my organization, job candidates, and friends who aren’t in the technology industry. To those of you who have asked me this question, I hope this is an acceptable response. For those who have arrived here through other means, welcome! Below is my attempt at describing what data engineering is, what skills a data engineer needs, and how it differs from data science. Things will be wrapped up with a look at opinions that I have developed about the job market for a data engineer.

###Data Engineer: Curator of Data
In short, a data engineer develops and maintains data pipelines in order to deliver data in an optimal format for a desired use. The role sits somewhere between a backend engineer and a data scientist. In some organizations, a data engineer will spend their days performing database design. In other organizations, time may be focused on developing and tweaking machine learning algorithms. In any case, a data engineer is tasked with enriching the data that is available to them.

Let's dig a little deeper into the short description I provided for a data engineer:

I mentioned that a data engineer develops and maintains data pipelines. Many of you are probably scratching your head about what is meant by *data pipeline*. A data pipeline is a series of steps that data goes through. Some of these steps are messaging mechanisms like an MQ service. Other steps are custom made processors that manipulate data before moving the data along to the next step in the sequence. It is up to the data engineer to know what the sequence of steps is and, when necessary, add steps to accomplish new goals.

What exactly is meant by an *optimal format for a desired use*? There are transformations that need to be made to many data sets in order for an analyst to use them. Sometimes the data has gaps that need to be filled in and other times the data is in XML format when it should be setup as a CSV. It is up to the data engineer to determine what the data will be used for, figure out the requirements for the output, and build a system to deliver on those requirements. After going through the stakeholder interview process, you may determine that all you need to do is write a 5-line BASH script. Alternatively, you may determine that you have to design and implement learning algorithm to infer missing information.

###Required Skills
* **Programming** - At the very least, a data engineer will be manipulating data with scripts. Even more likely, a data engineer will use concurrency and distributed systems to achieve high throughput. It takes many years to build up to the latter, but the knowledge is obtainable through many wonderful books and blogs.
* **Database Design and Tuning** - The data has to be stored somewhere. A good data engineer knows when they should use an OLTP design over an OLAP design, NoSQL over SQL, and a columnar database over a row-oriented database, to name a few decisions. A data engineer should also be able to effectively leverage features of various database systems to improve read and write performance.
* **Systems Design** - A data engineer will be tasked with building data pipeline systems. For a more junior engineer, this may be a single component in a large-scale data pipeline. For a senior engineer, this may involve architecting the entire large-scale pipeline.
* **Desire to Constantly Learn** - You will never know all of the libraries and systems that can be used to improve your data pipeline; there's too many of them. However, that shouldn't stop you from trying. 'Learn something new every day' should be the mantra of every data engineer. If you aren't learning, you aren't providing the most value possible to your team.

###Data Engineering vs. Data Science
The role of the data scientist has been glamorized over the last few years through the press received from major publications. This has led to many academies offering coursework in data science. With these events, the number of data scientists has grown significantly while data engineering has grown at normal rates. For this reason, data scientists are more frequently found in the wild than data engineers.

As I mentioned above, in most organizations, data engineers are responsible for collecting, cleaning, and organizing data. The work of a data engineer typically prepares data for a data scientist to begin the process of gaining valuable insights. A data engineer's work doesn't make much sense without having a data scientist or analyst to make use of the data. A data scientist isn't able to be as effective without having a data engineer to put the data in place.

It is important to mention that there is usually significant overlap in duties between a data engineer and a data scientist. For example, at LearnVest, our data scientists often perform some of their own data munging to convert raw data into valuable formats to have quick turnaround times when the data engineering team is swamped. The data engineers tend to pull reports for different business units in the organization to lend a helping hand to the data scientists and analysts.

###The Job Market
If you perform a search for 'data engineer' in New York City on Indeed, you will find, at the time of this writing, 1,200+ positions available. As data collection becomes easier, the volume, variety, and velocity of that data continues to increase. This requires data engineers to build the next generation of data processors and storage mechanisms. I expect the market for data engineers to continue to grow more rapidly than for data scientists. Many of these jobs will be labeled as software engineering jobs because it is easier to find software engineers than it is data engineers.

Speaking of the job market, [here's](http://hire.jobvite.com/m?37CL2hwi) the data engineering position that is the best (in my opinion)! At LearnVest, we are tackling a massive data pipeline project and would love to have another talented engineer join our ranks.