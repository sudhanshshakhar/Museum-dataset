<h2> # Demo Projects</h2>
<p> <h3>This is a demo project for a museum painting dataset and I'll evaluate the following requirements with SQL queries.</h3> 
<li> Fetch all paintings which are not displayed in any museum </li>
<li>Are there any museums without paintings</li>
<li>How many paintings have an asking price of more than regular price</li>
<li>Identify paintings whose asking price is less than 50% of their regular price </li>
<li>Which canvas size cost most</li>
<li>Delete duplicate records from work, product-size, subject, and image link tables</li>
<li>Identify the museum with invalid city information in the given dataset</li>
<li>Check the museum_hours table and find the invalid entity, identify it, and remove it.</li>
<li>Fetch top 10 most famous painting subjects </li>
<li>Identify the museum which is open on both Sunday and Monday. Display museum name, city</li>
<li>How many museums are open every single day</li>
<li>Which are the top 5 most popular museums? (Popularity is defined as based on most no. of paintings in the museum) </li>
<li>Which are the top 5 most popular museums? (Popularity is defined as based on most no. of paintings done by an artist</li>
<li>Display at least 3 popular canvas sizes </li>
<li>Which museum is open for the longest during the day - Display name, state, and hour open and which day?</li>
<li>Identify the artist whose paintings are displayed in multiple countries</li>
<li>Display the country and the city with the most no. of museums output two separate columns to mention the city and country. If there are multiple value, separate them with comma.</li>
<li>Which country has 5th highest no. of paintings</li>
<li>Which are the 3 most popular and 3 least popular painting styles?</li>
<li>Which artist has the most no. of painting outside the USA? Display the artist's name, no. of painting, and the artist's nationality.</li>

<h1>Schema<h2>
<h2>List of Column Names from all tables </h2>

<b>artist</b>- 
artist_id , full_name , first_name , middle_names , last_name , nationality ,style , birth , death

<b>canvas_size</b>- 
size_id , width , height , label

<b>image_link</b>- 
work_id , url , thumbnail_small_url , thumbnail_large_url

<b>museum</b>- 
museum_id , name , address , city , state , postal , country , phone , url

<b>museum_hours</b>- 
museum_id , day , open , close

<b>product_size</b>- 
work_id , size_id , sale_price , regular_price

<b>subject</b>- 
work_id , subject

<b>work</b>- 
work_id , name , artist_id , style , museum_id

