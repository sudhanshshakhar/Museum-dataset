<p> <h3>This is a demo project for a museum painting dataset.</h3>
<li> Fetch all paintings which are not displayed in any museum </li>
<li>Are there any museums without paintings</li>
<li>How many paintings have an asking price of less than regular price</li>
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

<h2><b>Schema and ERF</b></h2> (Table and column name/def.)

artist
- 
`artist_id` int PK FK >- work.artist_id</br>
`full_name` text </br>
`first_name` text</br>
`middle_names` text</br>
`last_name` text</br>
`nationality` text</br>
`style` text</br>
`birth` int</br>
`death` int</br>

canvas_size
-
`size_id` int PK FK >- product_size.size_id</br>
`width` int </br>
`height` text </br>
`label` text</br>

image_link
-
`work_id` int</br>
`url` text </br>
`thumbnail_small_url` text </br>
`thumbnail_large_url` text</br>

museum
-
`museum_id` int PK FK >- museum_hours.museum_id</br>
`name` text </br>
`address` text </br>
`city` text </br>
`state` text </br>
`postal` text </br>
`country` text </br>
`phone` text </br>
`url` text</br>

museum_hours
-
`museum_id` int FK >- work.museum_id</br>
`day` text</br>
`open` text </br>
`close` text</br>

product_size
-
`work_id` int PK FK >- image_link.work_id </br>
`size_id` int </br>
`sale_price` int </br>
`regular_price` int</br>

subject
-
`work_id` int PK FK >- image_link.work_id</br>
`subject` text</br>

work
-
`work_id` int PK FK >- subject.work_id</br>
`name` text </br>
`artist_id` int </br>
`style text` </br>
`museum_id` int</br>

![Screenshot 2024-03-08 134304](https://github.com/sudhanshshakhar/Museum_dataset_SQL/assets/159720338/fe6f8859-b59c-4c92-a45b-89a021ffdd4f)



