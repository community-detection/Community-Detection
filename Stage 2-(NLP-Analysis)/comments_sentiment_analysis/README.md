# Sentiment-Analysis

We chose two options to apply sentiment analysis on YouTube comments

The first option was TextBlob which is built on top of NLTK, and it’s more easily accessible. The other one is Stanford’s CoreNLP which is a Java library with Python wrappers. It’s in many existing production systems due to its speed.

The main differences between them were that Textblob does not compute the sentiment for emojis while Stanford corenlp compute it. Computing sentiment value for emojis is very important when analyzing the comments because most users when writing a comment use emojis 

The below table shows the percentages for positive/negative/neutral when using textblob and Stanford corenlp
<table>
  <tr>
    <th>Library Type</th>
    <th>Positive</th>
    <th>Neutral</th>
    <th>Negative</th>
  </tr>
  <tr>
    <td>Textblob</td>
    <td>0.46</td>
    <td>0.38</td>
    <td>0.14</td>
  </tr>
  <tr>
    <td>Stanford Corenlp</td>
    <td>0.22</td>
    <td>0.53</td>
    <td>0.20</td>
  </tr>
</table>




![](stage2b.png)
