---
layout: workshop      # DON'T CHANGE THIS.
carpentry: ""
venue: "R for Data Science"
address: "UCHC Center for Quantitative Medicine, 195 Farmington Ave, Farmington CT"
country: "us"
language: "en"
latlng: "41.7382143,-72.7936254"
humandate: "Wednesdays from May 1 - June 12, 2019"
humantime: "9:00 am - 12:30 pm"
startdate: 2019-05-01
enddate:  2019-06-12
instructor: ["Harshpreet Chandok", "Sue McClatchy", "Neil Kindlon", "Samir Amin", "Preeti Bais", "Ravi Pandey", "Pariksheet Nanda", "Lucas Lochovsky"]
helper: ["Annat Haber"]  
email: ["susan.mcclatchy@jax.org"]
collaborative_notes:  https://pad.carpentries.org/2019-05-01-r-for-data-science-ct
eventbrite: 60535875433
---

{% comment %} See instructions in the comments below for how to edit specific sections of this workshop template. {% endcomment %}

{% comment %}
HEADER

Edit the values in the block above to be appropriate for your workshop.
If the value is not 'true', 'false', 'null', or a number, please use
double quotation marks around the value, unless specified otherwise.
And run 'make workshop-check' *before* committing to make sure that changes are good.
{% endcomment %}

{% comment %}
EVENTBRITE

This block includes the Eventbrite registration widget if
'eventbrite' has been set in the header.  You can delete it if you
are not using Eventbrite, or leave it in, since it will not be
displayed if the 'eventbrite' field in the header is not set.
{% endcomment %}
{% if page.eventbrite %}
<iframe
  src="https://www.eventbrite.com/tickets-external?eid={{page.eventbrite}}&ref=etckt"
  frameborder="0"
  width="100%"
  height="280px"
  scrolling="auto">
</iframe>
{% endif %}


<h2 id="general">General Information</h2>

{% comment %}
INTRODUCTION

Edit the general explanatory paragraph below if you want to change
the pitch.
{% endcomment %}
This intermediate R series follows _R for Data Science_ by Hadley Wickham and Garrett Grolemund of RStudio. This series will teach you how to do data science with R. You’ll learn how to transform, visualize and model your data. You’ll learn how to use the grammar of graphics, literate programming, and reproducible research to save time. If you have already taken our R for Reproducible Scientific Analysis workshop, you meet the prerequisite for this course.

{% comment %}
AUDIENCE

Explain who your audience is.  (In particular, tell readers if the
workshop is only open to people from a particular institution.
{% endcomment %}
This series is open to those from UCHC, UConn, and JAX who meet the prerequisite for competence with R.

{% comment %}
LOCATION

This block displays the address and links to maps showing directions
if the latitude and longitude of the workshop have been set.  You
can use https://itouchmap.com/latlong.html to find the lat/long of an
address.
{% endcomment %}
{% if page.latlng %}
<p id="where">
  <strong>Where:</strong>
  {{page.address}}.
  Get directions with
  <a href="//www.openstreetmap.org/?mlat={{page.latlng | replace:',','&mlon='}}&zoom=16">OpenStreetMap</a>
  or
  <a href="//maps.google.com/maps?q={{page.latlng}}">Google Maps</a>.
</p>
{% endif %}

{% comment %}
DATE

This block displays the date and links to Google Calendar.
{% endcomment %}
{% if page.humandate %}
<p id="when">
  <strong>When:</strong>
  {{page.humandate}}.
  {% include workshop_calendar.html %}
</p>
{% endif %}

{% comment %}
SPECIAL REQUIREMENTS

Modify the block below if there are any special requirements.
{% endcomment %}
<p id="requirements">
  <strong>Requirements:</strong> Participants must bring a laptop with a
  Mac, Linux, or Windows operating system (not a tablet, Chromebook, etc.). They should have a few specific software packages installed (listed <a href="#setup">below</a>).
</p>

{% comment%}
CODE OF CONDUCT
{% endcomment %}
<p id="code-of-conduct">
<strong>Code of Conduct:</strong>  Everyone who participates  is required to conform to the <a href="https://docs.carpentries.org/topic_folders/policies/code-of-conduct.html">Code of Conduct</a>.
</p>


{% comment %}
ACCESSIBILITY

Modify the block below if there are any barriers to accessibility or
special instructions.
{% endcomment %}
<p id="accessibility">
  <strong>Accessibility:</strong> We are committed to making this workshop
  accessible to everybody.
  The workshop organizers have checked that:
</p>
<ul>
  <li>The room is wheelchair / scooter accessible.</li>
  <li>Accessible restrooms are available.</li>
</ul>
<p>
  Materials will be provided in advance of the workshop and
  large-print handouts are available if needed by notifying the
  organizers in advance.  If we can help making learning easier for
  you (e.g. sign-language interpreters, lactation facilities) please
  get in touch (using contact details below) and we will
  attempt to provide them.
</p>

{% comment %}
CONTACT EMAIL ADDRESS

Display the contact email address set in the configuration file.
{% endcomment %}
<p id="contact">
  <strong>Contact</strong>:
  Please email
  {% if page.email %}
  {% for email in page.email %}
  {% if forloop.last and page.email.size > 1 %}
  or
  {% else %}
  {% unless forloop.first %}
  ,
  {% endunless %}
  {% endif %}
  <a href='mailto:{{email}}'>{{email}}</a>
  {% endfor %}
  {% else %}
  to-be-announced
  {% endif %}
  for more information.
</p>

<hr/>

{% comment %} 
SURVEYS - DO NOT EDIT SURVEY LINKS 
{% endcomment %}
<h2 id="surveys">Surveys</h2>
<p>Please be sure to complete these surveys before and after the workshop.</p>

<p><a href="https://www.surveymonkey.com/r/r4ds-pre">Pre-workshop Survey</a></p>
<p><a href="https://www.surveymonkey.com/r/r4ds-post">Post-workshop Survey</a></p>

<hr/>


{% comment %}
SCHEDULE

Show the workshop's schedule.  Edit the items and times in the table
to match your plans.  You may also want to change 'Day 1' and 'Day
2' to be actual dates or days of the week.
{% endcomment %}
<h2 id="schedule">Schedule</h2>

<div class="row">
<div class="col-md-6">
<h3>Wednesday, May 1</h3>
<table class="table table-striped">
<tr> <td>9:00</td>  <td><a href="https://r4ds.had.co.nz/">Welcome and introductions</a></td> </tr>
<tr> <td>9:15</td>  <td><a href="https://r4ds.had.co.nz/explore-intro.html">Introduction to Data Exploration</a></td> </tr>
<tr> <td>9:55</td>  <td><a href="https://r4ds.had.co.nz/data-visualisation.html">Data Visualisation</a></td> </tr>
<tr> <td>10:45</td>  <td>Coffee</td> </tr>
<tr> <td>11:00</td>  <td><a href="https://r4ds.had.co.nz/data-visualisation.html">Data Visualisation (continued)</a></td> </tr>
<tr> <td>12:25</td>  <td>Wrap-up</td> </tr>
<tr> <td>12:30</td>  <td>End</td> </tr>
</table>
</div>
<div class="col-md-6">
<h3>Wednesday, May 8</h3>
<table class="table table-striped">
<tr> <td>9:00</td>  <td><a href="https://r4ds.had.co.nz/workflow-basics.html">Workflow: basics</a></td> </tr>
<tr> <td>9:30</td>  <td><a href="https://r4ds.had.co.nz/transform.html">Data Transformation</a></td> </tr>
<tr> <td>10:45</td>  <td>Coffee</td> </tr>
<tr> <td>11:00</td>  <td><a href="https://r4ds.had.co.nz/transform.html">Data Transformation (continued)</a></td> </tr>
<tr> <td>12:25</td>  <td>Wrap-up</td> </tr>
<tr> <td>12:30</td>  <td>End</td> </tr>
</table>
</div>
</div>
<div class="row">
<div class="col-md-6">
<h3>Wednesday, May 15</h3>
<table class="table table-striped">
<tr> <td>9:00</td>  <td><a href="https://r4ds.had.co.nz/workflow-scripts.html">Workflow: scripts</a></td> </tr>
<tr> <td>9:30</td>  <td><a href="https://r4ds.had.co.nz/exploratory-data-analysis.html">Exploratory Data Analysis</a></td> </tr>
<tr> <td>10:45</td>  <td>Coffee</td> </tr>
<tr> <td>11:00</td>  <td><a href="https://r4ds.had.co.nz/exploratory-data-analysis.html">Exploratory Data Analysis (continued)</a></td> </tr>
<tr> <td>11:25</td>  <td><a href="https://r4ds.had.co.nz/workflow-projects.html">Workflow: projects</a></td> </tr>
<tr> <td>11:40</td>  <td>Wrap-up</td> </tr>
<tr> <td>11:45</td>  <td>End</td> </tr>
</table>
</div>
<div class="col-md-6">
<h3>Wednesday, May 22</h3>
<table class="table table-striped">
<tr> <td>9:00</td>  <td><a href="https://r4ds.had.co.nz/wrangle-intro.html">Introduction to Data Wrangling</a></td> </tr>
<tr> <td>9:45</td>  <td><a href="https://r4ds.had.co.nz/tibbles.html">Tibbles</a></td> </tr>
<tr> <td>10:00</td>  <td><a href="https://r4ds.had.co.nz/data-import.html">Data Import</a></td> </tr>
<tr> <td>10:45</td>  <td>Coffee</td> </tr>
<tr> <td>11:00</td>  <td><a href="https://r4ds.had.co.nz/tidy-data.html">Tidy Data</a></td> </tr>
<tr> <td>12:25</td>  <td>Wrap-up</td> </tr>
<tr> <td>12:30</td>  <td>End</td> </tr>
</table>
</div>
</div>
<div class="row">
<div class="col-md-6">
<h3>Wednesday, May 29</h3>
<table class="table table-striped">
<tr> <td>9:00</td>  <td><a href="https://r4ds.had.co.nz/relational-data.html">Relational Data</a></td> </tr>
<tr> <td>10:15</td>  <td><a href="https://r4ds.had.co.nz/strings.html">Strings</a></td> </tr>
<tr> <td>10:45</td>  <td>Coffee</td> </tr>
<tr> <td>11:00</td>  <td><a href="https://r4ds.had.co.nz/strings.html">Strings (continued)</a></td> </tr>
<tr> <td>12:25</td>  <td>Wrap-up</td> </tr>
<tr> <td>12:30</td>  <td>End</td> </tr>
</table>
</div>
<div class="col-md-6">
<h3>Wednesday, June 5</h3>
<table class="table table-striped">
<tr> <td>9:00</td>  <td><a href="https://r4ds.had.co.nz/factors.html">Factors</a></td> </tr>
<tr> <td>10:15</td>  <td><a href="https://r4ds.had.co.nz/dates-and-times.html">Dates and Times</a></td> </tr>
<tr> <td>10:45</td>  <td>Coffee</td> </tr>
<tr> <td>11:00</td>  <td><a href="https://r4ds.had.co.nz/program-intro.html">Introduction to Programming</a></td> </tr>
<tr> <td>11:30</td>  <td><a href="https://r4ds.had.co.nz/pipes.html">Pipes</a></td> </tr>
<tr> <td>12:00</td>  <td><a href="https://r4ds.had.co.nz/functions.html">Functions</a></td> </tr>
<tr> <td>12:25</td>  <td>Wrap-up</td> </tr>
<tr> <td>12:30</td>  <td>End</td> </tr>
</table>
</div>
</div>
<div class="row">
<div class="col-md-6">
<h3>Wednesday, June 12</h3>
<table class="table table-striped">
<tr> <td>9:00</td>  <td><a href="https://r4ds.had.co.nz/vectors.html">Vectors</a></td> </tr>
<tr> <td>10:20</td>  <td><a href="https://r4ds.had.co.nz/iteration.html">Iteration</a></td> </tr>
<tr> <td>10:45</td>  <td>Coffee</td> </tr>
<tr> <td>11:00</td>  <td><a href="https://r4ds.had.co.nz/model-intro.html">Introduction to Modelling</a></td> </tr>
<tr> <td>11:30</td>  <td><a href="https://r4ds.had.co.nz/model-basics.html">Model Basics</a></td> </tr>
<tr> <td>12:00</td>  <td><a href="https://r4ds.had.co.nz/model-building.html">Model Building</a></td> </tr>
<tr> <td>12:25</td>  <td>Wrap-up</td> </tr>
<tr> <td>12:30</td>  <td>End</td> </tr>
</table>
</div>
</div>


{% comment %}
Collaborative Notes

If you want to use an Etherpad, go to

http://pad.carpentries.org/YYYY-MM-DD-site

where 'YYYY-MM-DD-site' is the identifier for your workshop,
e.g., '2015-06-10-esu'.
{% endcomment %}
{% if page.collaborative_notes %}
<p id="collaborative_notes">
  We will use this <a href="{{page.collaborative_notes}}">collaborative document</a> for chatting, taking notes, and sharing URLs and bits of code.
</p>
{% endif %}

<hr/>

{% comment %}
SYLLABUS

Show what topics will be covered.

1. If your workshop is R rather than Python, remove the comment
around that section and put a comment around the Python section.
2. Some workshops will delete SQL.
3. Please make sure the list of topics is synchronized with what you
intend to teach.
4. You may need to move the div's with class="col-md-6" around inside
the div's with class="row" to balance the multi-column layout.

This is one of the places where people frequently make mistakes, so
please preview your site before committing, and make sure to run
'tools/check' as well.
{% endcomment %}
<h2 id="syllabus">Syllabus</h2>

<div class="row">
<div class="col-md-6">
<h3 id="syllabus-r">Data Science in R</h3>
<ul>
<li>Reading and Plotting Data</li>
<li>Creating New Variables and Summaries</li>
<li>Generating Questions and Insights from Data</li>
<li>Working with Vectors and Tibbles</li>
<li>Working with Different Data Types</li>
<li>Building Models</li>
<li><a href="https://r4ds.had.co.nz/index.html">Reference...</a></li>
</ul>
</div>
</div>

<hr/>

{% comment %}
SETUP

Delete irrelevant sections from the setup instructions.  Each
section is inside a 'div' without any classes to make the beginning
and end easier to find.

This is the other place where people frequently make mistakes, so
please preview your site before committing, and make sure to run
'tools/check' as well.
{% endcomment %}

<h2 id="setup">Setup</h2>

<p>
  To participate in a
  {% if page.carpentry == "swc" %}
  Software Carpentry
  {% elsif page.carpentry == "dc" %}
  Data Carpentry
  {% elsif page.carpentry == "lc" %}
  Library Carpentry
  {% endif %}
  workshop,
  you will need access to the software described below.
  In addition, you will need an up-to-date web browser.
</p>
<p>
  We maintain a list of common issues that occur during installation as a reference for instructors
  that may be useful on the
  <a href = "{{site.swc_github}}/workshop-template/wiki/Configuration-Problems-and-Solutions">Configuration Problems and Solutions wiki page</a>.
</p>

<div id="r"> {% comment %} Start of 'R' section. {% endcomment %}
  <h3>R</h3>

  <p>
    <a href="https://www.r-project.org">R</a> is a programming language
    that is especially powerful for data exploration, visualization, and
    statistical analysis. To interact with R, we use
    <a href="https://www.rstudio.com/">RStudio</a>.
  </p>

  <div>
    <ul class="nav nav-tabs nav-justified" role="tablist">
      <li role="presentation" class="active"><a data-os="windows" href="#rstats-windows" aria-controls="Windows" role="tab" data-toggle="tab">Windows</a></li>
      <li role="presentation"><a data-os="macos" href="#rstats-macos" aria-controls="MacOS" role="tab" data-toggle="tab">MacOS</a></li>
      <li role="presentation"><a data-os="linux" href="#rstats-linux" aria-controls="Linux" role="tab" data-toggle="tab">Linux</a></li>
    </ul>
    <div class="tab-content">
      <article role="tabpanel" class="tab-pane active" id="rstats-windows">
        <a href="https://www.youtube.com/watch?v=q0PjTAylwoU">Video Tutorial</a>
        <p>
          Install R by downloading and running
          <a href="https://cran.r-project.org/bin/windows/base/release.htm">this .exe file</a>
          from <a href="https://cran.r-project.org/index.html">CRAN</a>.
          Also, please install the
          <a href="https://www.rstudio.com/products/rstudio/download/#download">RStudio IDE</a>.
          Note that if you have separate user and admin accounts, you should run the 
          installers as administrator (right-click on .exe file and select "Run as 
          administrator" instead of double-clicking). Otherwise problems may occur later, 
          for example when installing R packages.
        </p>
      </article>
      <article role="tabpanel" class="tab-pane active" id="rstats-macos">
        <a href="https://www.youtube.com/watch?v=5-ly3kyxwEg">Video Tutorial</a>
        <p>
          Install R by downloading and running
          <a href="https://cran.r-project.org/bin/macosx/R-latest.pkg">this .pkg file</a>
          from <a href="https://cran.r-project.org/index.html">CRAN</a>.
          Also, please install the
          <a href="https://www.rstudio.com/products/rstudio/download/#download">RStudio IDE</a>.
        </p>
      </article>
      <article role="tabpanel" class="tab-pane active" id="rstats-linux">
        <p>
          You can download the binary files for your distribution
          from <a href="https://cran.r-project.org/index.html">CRAN</a>. Or
          you can use your package manager (e.g. for Debian/Ubuntu
          run <code>sudo apt-get install r-base</code> and for Fedora run
          <code>sudo dnf install R</code>).  Also, please install the
          <a href="https://www.rstudio.com/products/rstudio/download/#download">RStudio IDE</a>.
        </p>
      </article>
    </div>
  </div>
</div> {% comment %} End of 'R' section. {% endcomment %}
