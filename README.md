<html>
	<head>
		<title>Hotel Reservation System</title>
		<style>
		body {background-color:rgb(250,250,250);}
		
		h1, h2, h3 {font-family: sans-serif;}
		
		.section_0{background-color:lightyellow;}
		.section_01{background-color:#FFD580;}
		.section_1{ background-color:powderblue;}
		.section_2{ background-color:lightgreen;}
			
		</style>

	</head>
	<body>
	
		<div class= "section_0">
		<font size="8">Hotel Reservation System</font>
		<!-- Reference a section within same HTML page + unordered_list -->
		<marquee>
				<!-- Greeting script based on time of day  -->
				<script>
				
				/* this is a comment for JavaScript*/
					var today= new Date();
					var hourNow= today.getHours();
					var greeting; 
					
					if(hourNow > 18){
					greeting = 'Good Evening from ';
					}else if (hourNow > 12){
					greeting = 'Good Afternoon from ';
					}else if (hourNow >0){
					greeting = 'Good morning from ';
					}else {
					greeting= "Welcome to "}
					document.write('<font size="18">' +greeting+'<i><b><span style="color: red">Fredi s Hotel</span></b></i> Reservation System</font>')
								  
				</script>
				
		</marquee>
	
		<!-- Image Banner-->
		<img src="Homepage_picture.PNG" alt="Vlore Albania" width="1240"/> <br/>
		<figcaption> Vlore, Albania </figcaption>
		
		</div>
		
		
		<!-- Reference a section within same HTML page + unordered_list -->
		<div class="section_01">

		<h2>Jump to a particular section </h2>
		<ul>
		<li><a href= "#reservation_section"> Reservation Section </a></li> 
	    <li><a href= "#calendar_section"> Calendar Section </a><br/> </li>
		</ul>  <br/>
		</div>
		
		<!-- Reservation -->
		<div class="section_1">
		<h2 id="reservation_section"> Reservation Section </h2>
		<p> In here we're going to have the reservation input from the user; most likely an in date and an out date, that will be followed by a confirmation button with user identifier (e.g. name)</p> <br/>
		
		<!-- Reservation_user information  -->
		<h3 id="reservation_user_input"> User Information </h3>
		<p> In here we're going to have the user information</p> <br/> 
		
		<table border="1">
			<tr> 
				<th colspan="2" width="600"> User Details </th>		
			</tr>
			<tr> 
				<th> Name:  </th>
				<td> <form> <input type="text" name="user_name" size="65"></form> </td>
			</tr>
			<tr> 
				<th> Last Name:  </th>
				<td> <form> <input type="text" name="user_lastname" size="65" ></form> </td>

			</tr>
			<tr> 
				<th> Phone Number: </th>
				<td> <form> <input type="text" name="user_phonenumber" size="65"></form> </td>

			</tr>
			<tr> 
				<th> Hotel Name Name: </th>
				<td> <form> <input type="text" name="hotel_id" size="65"></form> </td>

			</tr>
			<tr> 
				<th> Extra Comments: </th>
				<td> <form> <textarea name="comments" rows="4" cols="61"> </textarea> </form> </td>

			</tr>

		</table>
		
		<!-- Reservation_user stay dates  -->
		<h3 id="reservation_user_stay_dates"> Prenotation Dates </h3>
		<p> In here we're going to have the prenotation dates- meaning the days that the user will occupy the hotel. </p>
		
		<ul> 
			<li> <i>Arrival date</i>: is the day when the user will come to the hotel (first day)</li>
			<li> <i>Departure date</i>: is the day when the user will leave to the hotel (last day)</li>

		</ul>
		</br>
		<fieldset>
			<legend> Prenotations Dates</legend>
				<form> 
					<label for="user_name"> <b>Arrival Date:  </b></label>
					<input type="date" name= "arrival"/>
				    <label for="user_name"> <b>Departure Date:  </b></label>
					<input type="date" name= "Departure"/>
					<input type="submit" name= "confirmation_button" value="Confirm Prenotation Dates"/>

				</form>

		</fieldset>
	    
		</div>

		<div class="section_2">
		<!-- Calendar -->
		<h2 id= "calendar_section"> Calendar Section</h2>
		<p>In here we're going to display the calendar with the appropriate reservations showing. </p> <br/> <br/>
		
		<!-- Table , hard corded -->
		<table border="1">
		<thead>
			<tr> 
			<th> Month: April </th>
			
			</tr>
			<tr> 
				<th> Sunday </th>
				<th> Monday </th>
				<th> Tuesday </th>
				<th> Wednesday </th>
				<th> Thursday </th>
				<th> Friday </th>
				<th> Saturday </th>
			</tr>
			
		</thead>
		<tbody>
			<tr> 
				<td> 1 </td>
				<td> 2</td>
				<td> 3</td>
				<td> 4</td>
				<td> 5</td>
				<td> 6</td>
				<td> 7</td>
			</tr>
			<tr> 
				<td> 8 </td>
				<td> 9</td>
				<td> 10</td>
				<td> 11</td>
				<td> 12</td>
				<td> 13</td>
				<td> 14</td>
			</tr>
			<tr> 
				<td> 15 </td>
				<td> 16</td>
				<td> 17</td>
				<td> 18</td>
				<td> 19</td>
				<td> 20</td>
				<td> 21</td>
			</tr>
			<tr> 
				<td> 22 </td>
				<td> 23</td>
				<td> 24</td>
				<td> 25</td>
				<td> 26</td>
				<td> 27</td>
				<td> 28</td>
			</tr>
			<tr> 
				<td> 29 </td>
				<td> 30 </td>
				<td> </td>
				<td> </td>
				<td> </td>
				<td> </td>
				<td> </td>
			</tr>
		</tbody>
		</table>

		</br>
		
		</div>
		
		<div id="footer">
		<!-- Footer, include contact info -->
		<footer>
			<address> email: <a href="mailto:mzanaj@umich.edu"> mzanaj@umich.edu</a> <br>
			phone: <a href="">000-000-0000</a>
			</address>
		</footer>
		</div>
	</body>
</html>
 
# Welcome to Martin Zanaj's Github 

In this interface, you will find links to homeworks and projects that I have completed as a result of my master's degree in data science at the University of Michigan and more. The goal is to showcase the different topics and skills that I've been able to acquire and develop. Most of the work is indeed my own, but it is imperative to mention the many resources such as books, videos, and online documentation that I have resorted to in order to better my understanding and ultimately complete the assignments.  

## Master's Courses UMICH

**STATISTICAL LEARNING: LINEAR REGRESSION**

This course is an overview of Regression, and its application through R. This is a master's course. As a result, it attemps to cover both theory & practice with a depth that allows for a more than necessary understanding of liner models. This was my first encounter with R and Linear Regression. Perhaps, this is one of the topics I am most fond of given it was my introduction to the world  of data science- a "first love", so to speak.

| | |
|-|-|
|__Skills__| R, RMarkdown Reporting, Data Modeling & Analysis, Statistical Inference |
|__Topics__| linear regression, ANOVA, diagnostics, Huber's robust regression, LAD, model selection (Mallow's Cp, Adjusted R^2, Ridge, Lasso), Binomial & Poisson regression |
|__HW Repository__| https://github.com/mzanaj/Linear-Models-with-R |

   
**DATA SCIENCE AND ANALYTICS WITH PYTHON**

This course was my introduction to the world of Python and its popular packages. It surveyed some of the tools and frameworks currently popular among data scientists and machine learning practitioners in academia and industry. The first half of the course consisted of an accelerated introduction to the Python programming language, including brief introductions to object-oriented and functional programming styles as well as tools for code optimization. The second half of the course surveyed tools for handling structured data (regular expressions, HTML/JSON, databases), data visualization, numerical and symbolic computing, and large-scale distributed computing.

| | |
|-|-|
|__Skills__| Python, Jupyter, SQL |
|__Packages__| functools, itertools, numpy, pandas, matplotlib, re, urllib.request, sqlite3|
|__Topics__| functions, string/file/dataFrame manipulation, class, SQL Queries, time analysis|
|__HW Repository__| https://github.com/mzanaj/Data-Science-Aanalytics-with-Python |  
  

**INFORMATION VISUALIZATION**

Perhaps a course that thought me the meanining of "One picture a thousands words." The course focused on how to present information effectively and in an unbiased way. Often time one has to make trade-offs, and these trade-offs have to be according to the most imoprtant objective that your data/study aims at solving. More specifically, this course provides an in-depth introduction to the state-of-the-art in information visualization. Through a series of readings, videotapes, and discussions, students look at various strategies that have been developed, including their static, dynamic, and interactive aspects, and understand when, where, and why they work. In addition, there is an effort to place Information Visualization in the more general contexts of visualization (e.g., as used in statistics and physics) and information work. 

| | |
|-|-|
|__Skills__|Google Collab, Tableau, Altair, HTML |
|__Topics__| line charts, bar graphs, aesthetics, annotations, heatmaps, interactive visualizaations |
|__HW Repository__| https://github.com/mzanaj/Information-Visualization |  

| | |
|-|-|
|__Group Project__| Analysis of Planes Crashes|
|__Responsibility__| Chart 3. What are the most common causes of accidents? |
|__Repository__|https://elaineye117.github.io/flight_crash_analysis/ | 

| | |
|-|-|
|__Personal Project__| Election Results/Predictions |
|__Description__| In this project, I was required to develop an HTML webpage that included possible insights from the data (through visualization). The key idea was to create a story line, backed by data (Altair Charts) and present it to a less technical audience. The HTML files and as well a rendered PDF of the webpage can be accessed at the link below.   |
|__Repository__|https://github.com/mzanaj/Information-Visualization/tree/main/Personal%20Project | 


**APPLIED MACHINE LEARNING**

One of my favorite course where I was able to take the theory of statistical methods (mainly topics discussed in the book "An Introduction to Statistical Learning") and put it to practice by way of Python and its powerful machine learning libraries.  In this course, I solved supervised and unsupervised machine learning problems on real-world datasets. The class focuses more on application than theory and was based on the scikit-learn (for classical ML) and Keras (for Deep ML) libraries in Python. 

| | | 
|-|-|
|__Skills__| Data Analysis w/ supervised/unsupervised models |
|__Packages__|Scikit-learn, keras, numpy, pandas, matplotlib|
|__Topics__|  KNN, linear/poly/logisitics/LASSO/ridge regression, SVM, tree (Bagging, Random Forest,Boosting), Naive Bayes, deep learning, validation (CV, GS), regularization, metrics (accuracy, MSE, F1,..), ROC, AUC,one hot encoding |
|__HW Repository__| https://github.com/mzanaj/Applied-Machine-Learning |  
  
**DATA MINING**

This course was an introduction to the world of data mining, which I've come to recognize as "data through the eyes of a computer scientist". Although, this is a personal viewpoint, the course focused on how the information in different real-world problems can be represented as particular genres, or formats of data, and how the basic mining tasks of each genre of data can be accomplished using the state-of-the-art techniques. The list of topics in this course was massive (like the book itself "Mining Massive Datasets"),and as a result a one semester is not enough to master all of the concepts. Nevertheless, it was an important starting point that exposed me to previously unknown techniques. The course only had 3 different homeworks, but they were the longest homework I've encountered in my academic career. Altough the tasks were far from easy and trivial, at the end of each homework, I felt extremely accomplished and good about myself. 

| | | 
|-|-|
|__Skill__| Data Mining, Itemset Mining, Graph Analysis |
|__Packages__| pandas, matplotlib, seaborn, apyori, Scikit-learn, surprise, networkx,  |
|__Topics__| EDA, feature selection, dataFrame manipulation, apriori, SVD, graph/network, PageRank|
|__HW Repository__| https://github.com/mzanaj/Data-Mining |  

**NIH**
This repository will hold resources pertaining to the NIH-sponsored machine learning project that is being developed at Oregon State University.
| | | 
|-|-|
|__Skill__| Data Pre-processing|
|__Packages__| pandas, matplotlib, seaborn |
|__Topics__| EDA |
|__Repository__|https://github.com/mzanaj/NIH-Machine-Learning |  


**PERSONAL ENDEAVORS**

| |
|-|
|**Certifications**|
|These are certs that attest the completion of Data Camp courses. Data Camp is an online platform to develop DS skills| 
|Repository: https://github.com/mzanaj/Data-Camp|

| |
|-|
|**NLP**|
|A glimpse of the fascinating world of NLP.The material was developed for a seminar presentend to incoming freshman students| 
|Repository: https://github.com/mzanaj/NLP |

| |
|-|
|**Stats**|
|Important topic relevant to both fields of data science and statistics- a mix of theory and practice| 
|Repository: https://github.com/mzanaj/Statistics |

| |
|-|
|**Videos of me teaching**|
|Statistics lab: https://youtu.be/x-09VU-0Fwc| 
|Programming demo: https://youtu.be/ulIh7jSIo4E|
  
  
## Contact Info & Public Links

LinkedIn: www.linkedin.com/in/mzanaj

Personal Blog: https://mzanaj.blogspot.com/ 

Tableau Public: https://public.tableau.com/profile/martin6851#!/ 

Email: mzanaj@umich.edu 
