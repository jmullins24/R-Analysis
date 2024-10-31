<h1>R Analysis</h1>

<h2>Description</h2>
Assignment consisted of analyzing the dataset collected by political canvasing and testing the change in tolerance levels of transgender individuals based on having a short conversation with one versus receiving a control conversation about recycling. Analysis shows the treatment effect varies significantly across political and racial demographics.
<br />


<h2>Languages and Utilities Used</h2>

- <b>R Studio</b> 
- <b>Dplyr</b>
- <b>ggplot2</b>

<h2>Environments Used </h2>

- <b>Windows 11</b> (21H2)

<h2>Program walk-through:</h2>

<p align="center">
Code for : <br/>
<img src="https://i.imgur.com/Z22Y9to.jpeg" height="80%" width="80%" alt="R Code calculating means accross treatment and control group"/>
<br />
<br />
Graphing the Means:  <br/>
<img src="https://i.imgur.com/bMDtYt6.jpeg" height="80%" width="80%" alt="Graph showing difference in opinion on transgender issues based on treatment status"/>
<br />
<br />
Calculating correlations:  <br/>
<img src="https://i.imgur.com/ljkPR06.jpeg" height="80%" width="80%" alt="Correlation calculations"/>
<br />
<br />
Plot code:  <br/>
<img src="https://i.imgur.com/krJMLeo.jpeg" height="80%" width="80%" alt="ggplot"/>
<br />
<img src="https://i.imgur.com/znLfCiB.jpeg" height="80%" width="80%" alt="Correlation calculations"/>
<br />
<br />
Plots showing opinion variations by demographics:  <br/>
<img src="https://i.imgur.com/7e9fpoJ.jpeg" height="80%" width="80%" alt="Correlation calculations"/>
<br />
Do political parties respond differently to the treatment? Yes, the republicans were significantly less tolerant within the first 3 days of the treatment, while democrats were near 0 effect and independents were slightly positive. Republicans also ended the 90 days at a lower tolerance level than the other groups, and closer to the average population. Do racial groups react differently? Yes, while Caucasians and Hispanics had similar reactions over time, surprisingly, African Americans actually had an adverse reaction to the treatment. They ended up having less tolerance than average after the canvasing experience. Since the tolerance level is measured as standard deviations, 0 is the 50th percentil of the general population’s tolerance. Having a positive number means you are more tolerant than the average person, and negative means you are less so.
<br />
Average Treatment Effect code accounting for those who were assigned to each group but did not follow through:  <br/>
<img src="https://i.imgur.com/PWCZgLW.jpeg" height="80%" width="80%" alt="Correlation calculations"/>
<br />
<br />
Plot result:  <br/>
<img src="https://i.imgur.com/0QXTPay.jpeg" height="80%" width="80%" alt="Correlation calculations"/>
<br />
<br />
Did engagement vary by gender? No, not significantly. Both males and females were likely to respond 87% of the time they were approached.

Did engagement vary by political party? Yes, democrats were 3.5% more likely to answer than republicans and 7.5% more likely than independents.

Did engagement vary by race? Yes, African Americans were 7% more likely to answer than Hispanics and 7.9% more likely to answer than Caucasians.

What does this imply about the differences in question 1? Initially we calculated the ATE based on those who were assigned the treatment, and didn’t take into account those who actually received it. To establish strong conclusions, we need to calculate the treatment effect based on the people who actually received the treatment. Non-compliance with the treatment leads to uncertainty about whether the observed outcomes were a result of the treatment or not, which threatens the internal validity because we can’t clearly state the cause-effect relationship.

What does the complication imply when interpreting the results of question 1? Since some who were assigned did not comply with treatment, and some in the placebo group received it by mistake, it is likely that our estimate in question one was underestimating the treatment effect. There, we were calculating the tolerance levels of people in the ‘treatment group’ that hadn’t actually participated in the treatment activity, so their responses would have been more like the placebo’s responses.
<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
