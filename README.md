# cs253-assignment-2-solved
**TO GET THIS SOLUTION VISIT:** [CS253 Assignment 2 Solved](https://www.ankitcodinghub.com/product/cs253-assignment-2-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;98057&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS253 Assignment 2 Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

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

<div class="kksr-stars-active" style="width: 0px;">
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
            <span class="kksr-muted">Rate this product</span>
    </div>
    </div>
<div class="page" title="Page 1">
<div class="layoutArea">
<div class="column">
Assignment 2: Advanced Bash Scripting

We will be using the shell commands to accomplish a simple task here. The task is related to covid data extracted from www.covid19india.org. Download the json(you may use wget) from https://api.covid19india.org/v4/data.json. Name the file as covid_Data.json and place it in the home folder of the unzipped cs253_assign_2.zip.

Following is a small snippet showing how to access json data using jq(may have to install separately). Following is a sample json:

<pre>{
“A” : ”a”,
“B” : “b”,
“C” : “c”,
“D” : {
</pre>
“d” : “4”

} }

To retrieve the value “c” one way to get is: –

jq “.C|values” &lt;path_Of_The_JSON_File&gt; –output c To retrieve the value “4” we get it like this: –

jq “.D.d|values” &lt;path_Of_The_JSON_File&gt; –output 4

Task

Explore and access the downloaded covid_Data json file from within the solution shell file. Make a csv file named processed_Covid_Data_&lt;your_Roll_Number&gt;.csv. with the format as shown,

&lt;state&gt;, &lt;district&gt;, &lt;confirmed_Cases&gt;, &lt;recovery_Rate&gt; where,

<ul>
<li>state is the state code, example AN, KA etc.,</li>
<li>district is the district name with maximum recovery rate,</li>
<li>confirmed_Cases is the number of confirmed cases for this district name
<pre>      (district with max recovery rate),
</pre>
</li>
<li>recovery_Rate is the recovery rate for this district name (district with</li>
</ul>
</div>
</div>
<div class="layoutArea">
<div class="column">
Note:

</div>
<div class="column">
max recovery rate).

Recovery rate is calculated as [(recovered/confirmed) * 100]

Consider the following while performing the task:

</div>
</div>
<div class="layoutArea">
<div class="column">
• For every state code, consider districts with more than or equal to 5000 number of confirmed cases for processing, ignoring the rest.

</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
<ul>
<li>Avoid including the state code entry in csv, if the number of confirmed cases for all of its districts is less than 5000.</li>
<li>While processing, you may get “Unknown” as a district name, ignore the processing for that district. In the csv, we should not have “Unknown” as a district name for any state code.</li>
<li>Recovery rate may be equal for two districts, include the one in csv that comes later while processing. Example, for a state code(st), db district (98 percent recovery rate) and da (98 percent recovery rate) are there, csv should consist of da as the district name.</li>
<li>Ignore errors at any stage (you may create log file).</li>
<li>You may add headers to the generated csv file if you wish.
A csv file for a sample data on marks shown below, —————————————————————————–
</li>
</ul>
Name Marks_Sub_1 Marks_Sub_2 Preeti 25 31

Ravi 25 30

Ankit 24 31

—————————————————————————– looks like this,

<pre>Preeti,25,31
Ravi,25,30
Ankit,24,31
</pre>
</div>
</div>
</div>
