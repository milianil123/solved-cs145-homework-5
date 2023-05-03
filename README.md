Download Link: https://assignmentchef.com/product/solved-cs145-homework-5
<br>
<h1>1           Frequent Pattern Mining for Set Data</h1>

Given a transaction database shown in Table 1, answer the following questions. Note that the parameter min support is set as 2.

<ul>

 <li>Find all the frequent patterns using Apriori Algorithm. Details of the procedure are expected.</li>

 <li>Construct and draw the FP-tree of the transaction database.</li>

 <li>For the item <em>d</em>, show its conditional pattern base (projected database) and conditional FP-tree.</li>

 <li>Find frequent patterns based on <em>d</em>’s conditional FP-tree.</li>

</ul>

Table 1: The transaction database for the question 1.

<table width="106">

 <tbody>

  <tr>

   <td width="43">TID</td>

   <td width="63">Items</td>

  </tr>

  <tr>

   <td width="43">1</td>

   <td width="63"><em>b,c,j</em></td>

  </tr>

  <tr>

   <td width="43">2</td>

   <td width="63"><em>a,b,d</em></td>

  </tr>

  <tr>

   <td width="43">3</td>

   <td width="63"><em>a,c</em></td>

  </tr>

  <tr>

   <td width="43">4</td>

   <td width="63"><em>b,d</em></td>

  </tr>

  <tr>

   <td width="43">5</td>

   <td width="63"><em>a,b,c,e</em></td>

  </tr>

  <tr>

   <td width="43">6</td>

   <td width="63"><em>b,c,k</em></td>

  </tr>

  <tr>

   <td width="43">7</td>

   <td width="63"><em>a,c</em></td>

  </tr>

  <tr>

   <td width="43">8</td>

   <td width="63"><em>a,b,e,i</em></td>

  </tr>

  <tr>

   <td width="43">9</td>

   <td width="63"><em>b,d</em></td>

  </tr>

  <tr>

   <td width="43">10</td>

   <td width="63"><em>a,b,c,d</em></td>

  </tr>

 </tbody>

</table>

1

Introduction to Data Mining (UCLA CS 145)                                                                                            Homework #5

<h1>2           Apriori for Yelp</h1>

In apriori.py, fill in the missing lines, with the following parameters (already set in the code): min_support=50, min_conf=0.25, and ignore_one_item_set=True. Output the frequent patterns and rules associated with the Yelp data (the same one as the project) which we have stored in yelp.csv and id_name.csv. Do NOT modify the print_items_rules() function and directly copy the entire output of the following command in your report in plain text format (do NOT take a screenshot):

python2.7 apriori.py

What patterns and rules do you see? Where are these businesses located? What do these results mean? Do a quick Google search and briefly interpret the patterns and rules mined from Yelp in 50 words or less.

<h1>3           Correlation Analysis</h1>

Table 2 shows how many transactions containing beer and/or nuts among 10000 transactions. Answer the following questions based on Table 2.

<ul>

 <li>Calculate confidence, lift, and all confidence between buying beer and buying nuts.</li>

 <li>What are your conclusions of the relationship between buying beer and buying nuts, based on the above measures?</li>

</ul>

Table 2: Contingency table for question 2.

<table width="234">

 <tbody>

  <tr>

   <td width="69"> </td>

   <td width="45">Beer</td>

   <td width="68">No Beer</td>

   <td width="52">Totel</td>

  </tr>

  <tr>

   <td width="69">Nuts</td>

   <td width="45">150</td>

   <td width="68">700</td>

   <td width="52">850</td>

  </tr>

  <tr>

   <td width="69">No Nuts</td>

   <td width="45">350</td>

   <td width="68">8800</td>

   <td width="52">9150</td>

  </tr>

  <tr>

   <td width="69">Total</td>

   <td width="45">500</td>

   <td width="68">9500</td>

   <td width="52">10000</td>

  </tr>

 </tbody>

</table>

<h1>4           Sequential Pattern Mining (GSP Algorithm)</h1>

<ul>

 <li>For a sequence <em>s </em>= h<em>ab</em>(<em>cd</em>)(<em>ef</em>)i, how many events or elements does it contain? What is the length of <em>s</em>? How many non-empty subsequences does s contain?</li>

 <li>Suppose we have <em>L</em><sub>3 </sub>= {h(<em>ac</em>)<em>e</em>i<em>,</em>h<em>b</em>(<em>cd</em>)i<em>,</em>h<em>bce</em>i<em>,</em>h<em>a</em>(<em>cd</em>i<em>,</em>h(<em>ab</em>)<em>d</em>i<em>,</em>h(<em>ab</em>)<em>c</em>i} as the frequent 3sequences, write down all the candidate 4-sequences <em>C</em><sub>4 </sub>with the details of the join and pruning steps.</li>

</ul>

2