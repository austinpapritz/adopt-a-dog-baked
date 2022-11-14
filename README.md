# Rubric

Here is the model for the `dogs` table

![model of dogs table](./dogs-model.png)

| Tasks...                                                                                       | **10** |
| ---------------------------------------------------------------------------------------------- | ------ |
| ASYNC: `getDogs()` : return array of dogs from supabase                                        | 2      |
| On load on the home page, see a list of dogs (names and breed image), fetched from supabase    | 2      |
| On clicking a dog, user should be taken to that dog's detail page.                             | 2      |
| ASYNC: `getDog(id)` : return single dog from supabase                                          | 2      |
| Detail page should get the id from the URL and use that id to fetch that dog from supabase.    | 2      |
| Detail page should show the user details about the dog (including age, breed, and description) | 2      |

## HTML

-   Home Page:
    -   div to hold list of items
    -   render each item fetched from supabase
-   Detail Page:
    -   section and div container for details
    -   header: link back to homepage

## Events

-   home page load
    -   fetch items from supabase
    -   render items in cards
    -   display items
        -   loop through, append elements in render, append to container in DOM
-   detail page load
    -   fetch single item (by ID)
    -   render to page
    -   use URLSearchParams to get ID from URL

## Functions

-   fetch-utils.js: getDogs() getDogById()
-   render-utils.js: renderCards() renderDetails()

## Slices

1. get items to render on load
2. make cards clickable, redirecting to detail page
3. render appropriate details on detail page
4. use URLSearchParams to fill in id dynamically
