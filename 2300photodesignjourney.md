# Project 3: Design Journey

Be clear and concise in your writing. Bullets points are encouraged.

**Everything, including images, must be visible in VS Code's Markdown Preview.** If it's not visible in Markdown Preview, then we won't grade it.

# Design & Plan (Milestone 1)

## Describe your Gallery (Milestone 1)
> What will your gallery be about? 1 sentence.
My gallery will be photos from the two Disney theme parks I have been to: Florida and California.

> Will you be using your existing Project 1 or Project 2 site for this project? If yes, which project?
I will not be using an existing project.

> If using your existing Project 1 or Project 2, please upload sketches of your final design here.



## Target Audience(s) (Milestone 1)
> Tell us about your target audience(s).

The target audience are people who are planning to visit either of the Disney parks, whether Disney World in Florida, or Disneyland/Disney California Adventure in California. They might want to see images from the parks as well as some of the food that one could get there, and they may want to see what the atmosphere is like at those parks before they go there.

## Design Process (Milestone 1)
> Document your design process. Show us the evolution of your design from your first idea (sketch) to design you wish to implement (sketch). Show us the process you used to organize content and plan the navigation (card sorting), if applicable.
> Label all images. All labels must be visible in VS Code's Markdown Preview.
> Clearly label the final design.

preliminary sketch of the full gallery page
![](prelimgallery.png)


second preliminary sketch of the individual image page. I added a back button to go back to viewing the whole gallery. This page will include the description of the image as well. I also changed the way to remove a tag, by putting a "-" or a small trash can next to the list of tags on that image's tags page.
![](prelimimg2.png)


preliminary sketch of the individual image page
![](prelimimg.png)


preliminary sketch of the list of tags page
![](prelimtags.png)


second preliminary sketch of the list of tags page. it is more or less the same as the first preliminary sketch, except that I decided to change the style of the bullet points to a more open one.
![](prelimtags2.png)


preliminary sketch of the upload a new image page
![](prelimupload.png)



final sketch of the full gallery page. Instead of an "add photo" link in the navigation bar, I changed it to "upload", because it looks cleaner. I also decided to line up the photos differently and have them one at a time, because this way, the user could see the images at a bigger size and not have to try and guess what is in the photo by looking at a small thumbnail.
![](finalgallery.png)


final sketch of the individual clicked on image page. It has the same elements as the preliminary sketches, but I put the description, tags, etc on the side of the image instead of below it. This is because when the image is clicked on, the user may not see the description/etc and might think that nothing happened.
![](finalimg.png)


final sketch of the tags list page. I decided to change it from a bulleted list of points to the tags having their own boxes. I thought that this looked more aesthetically pleasing and fun, instead of just a long list.
![](finaltags.png)


final sketch of the upload a new image page. it is the same as the preliminary sketch.
![](finalupload.png)


## Design Patterns (Milestone 1)
> Explain how your site leverages existing design patterns for image galleries.
> Identify the parts of your design that leverage existing design patterns and justify their usage.
> Most of your site should leverage existing patterns. If not, fully explain why your design is a special case (you need to have a very good reason here to receive full credit).

The site leverages existing design patterns for image galleries because it has a "+" sign instead of the words "add tag" when a user wants to add a tag. I also would like to include either a "-" or a small trash can icon next to the list of an image's tags after the user clicks on it for further information. The "+" and the "x"/trash can are pretty constant throughout many platforms, as connotations for either adding or removing some kind of element from a site, so with these icons in my own site, it will be fairly easy for users to understand what they need to do.
However, in order to delete an image, I will not use a trash can or "-" for this. This is because there would already be this negative sign of removing something for the tags, so the user might get confused. It is also because if there was only a small icon underneath the text needed for a user to add a tag, the design would look unbalanced, and I didn't want that.


## Requests (Milestone 1)
> Identify and plan each request you will support in your design.
> List each request that you will need (e.g. view image details, view gallery, etc.)
> For each request, specify the request type (GET or POST), how you will initiate the request: (form or query string param URL), and the HTTP parameters necessary for the request.

Example:
- Request: view movie details
  - Type: GET
  - Params: id _or_ movie_id (movies.id in DB)

- Request: view images
  - Type: GET
  - Params: image name and id in DB

- Request: click on image to view more information
  - Type: form, get
  - Form

- Request: add/remove tags
  - Type: form, post
  - Params: image name, tag_id in DB

- Request: delete image
  - Type: form, post
  - Params: image_id, tag_id, tags in DB

- Request: upload file
  - Type: POST
  - Form

- Request: go back to the gallery page from the individual image's extra information page
  - Type: GET
  - Form


## Database Schema Design (Milestone 1)
> Plan the structure of your database. You may use words or a picture.
> Make sure you include constraints for each field.

> Hint: You probably need `images`, `tags`, and `image_tags` tables.

> Hint: For foreign keys, use the singular name of the table + _id. For example: `image_id` and `tag_id` for the `image_tags` table.

```
images (
    id: INTEGER {PK, U, Not, AI},
    file_name: TEXT {},
    file_ext: TEXT {},
    description: TEXT {}
)
```
```
tags (
    id: INTEGER {PK, U, Not, AI},
    tag: TEXT {}
)
```
```
image_tags (
     id: INTEGER {PK, U, Not, AI},
     image_id: INTEGER,
     tag_id: INTEGER
)
```


## Database Query Plan (Milestone 1)
> Plan your database queries. You may use natural language, pseudocode, or SQL.
> Using your request plan above, plan all of the queries you need.

view all of the images
```sql
SELECT * FROM images;
```

view only one of the photos
```sql
SELECT * FROM images WHERE images.id = ':images.id';
```

add a tag
```sql
INSERT INTO image_tags (image_id, tag_id) VALUES (':image_id', ':tag_id');
```

remove a tag
```sql
DELETE * FROM image_tags WHERE id = ':image_tags_id' AND 'image_id' = ':image_id';
```

add/upload image
```sql
INSERT INTO images (id, file_ext, description) VALUES (':id', ':file_ext', ':description');
```

delete an image
```sql
DELETE * FROM images WHERE images.id = ':images.id';
```


## Code Planning (Milestone 1)
> Plan what top level PHP pages you'll need.

index.php will be the homepage, and will include the entire gallery of images.
indiv_image.php will be the page that shows up when the user clicks on an image for further information.
tags.php will include a list of every single tag.
upload.php will be the page where the user will be able to upload images and add in a description.

> Plan what partials you'll need.

the partial that I will use will be a header that includes the words "Disney Photo Gallery" and the navigation bar.

> Plan any PHP code you'll need.

view all images:
  use the following sql --> SELECT * FROM images;

click on a photo for further information:
  echo the name of the image that was clicked on and change to that page
  show the tags for that image
  show the sql to remove the tag and delete the image

# Complete & Polished Website (Final Submission)

## Gallery Step-by-Step Instructions (Final Submission)
> Write step-by-step instructions for the graders.
> For each set of instructions, assume the grader is starting from index.php.

Viewing all images in your gallery:
1. scroll downwards, all images will be on the index.php page

View all images for a tag:
1. go to tags page from the navigation bar
2. click on a tag to see the photos

View a single image and all the tags for that image:
1. click on a photo from the index.php page

How to upload a new image:
1. go to upload page from the navigation bar
2. fill out the upload form, and press the upload button
3. go back to the index.php page, and the image will be there

How to delete an image:
1. click on photo from the index.php page
2. click on the delete photo button

How to view all tags at once:
1. go to tags page from the navigation bar

How to add a tag to an existing image:
1. click on photo from the index.php page
2. create a new tag by typing in the labelled textbox
3. click the "+" button next to said textbox
4. refresh the page to see the newly added tag

How to remove a tag from an existing image:
1. click on photo from the index.php page
2. click on the "x" button next to the tag that you want to delete


## Reflection (Final Submission)
> Take this time to reflect on what you learned during this assignment. How have you improved since starting this class?

I learned how to try and solve things on my own without heavily relying on office hours, or other people. I also learned a lot more about SQL queries, and how to use different things to maniupulate them, such as arrays or other functions like lastInsertId(). I've improved since starting the class by learning to how use PHP and SQL effectively. For example, in the beginning of the class, I was very confused about PHP echo, and how it could be used at all while being integrated into HTML that we already learned from 1300. However, by the end of this project, I found that I was able to use echo a lot more, and that it was actually very helpful, allowing me to do things that were much harder in 1300.
