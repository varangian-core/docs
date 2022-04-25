---
title: "Advanced Search"
date: 2022-04-18T16:35:16-07:00
weight: 5
---
### Advanced Search

There are many other ways to search for the documents that are available to advanced users:
- cabinets
- favorites
- tags
- workflows 
- checkouts
- whoosh search engine

So let's take a look at how these things work:

#### Searching by Cabinets

The user can file the document in the specific folder under `cabinets/details`

Certain users may create their own cabinet, and upload their own documents for individual use.

![Cabinet folders](images/temp_assets/cabinet_folders.PNG)    


#### Searching by Favorites
Each user has their own favorites folder located under `Documents` panel. A user may want to `favorite` a file in one of two ways:
![Favorites Folder](/images/temp_assets/favorites.png)
<br>
**Bulk Selection** </br>
Go to the documents folder and select multiple files by clicking on checkboxes. This will open bulk actions button in top right.
Select `add to favorites`.
![Bulk Add to Favorites](/images/temp_assets/bulk_add_to_favorites.png)
**File Selection**
By clicking on the file, you will get into the file menu. Under `actions` (top right corner button) you can select 'add to favorites'
![File Add to Favorites](/images/temp_assets/add_to_favorite.png)
#### Searching by Tags
Advanced users may also have access to item tags. Tags help place items into additional categories. 
![Tags](/images/temp_assets/tags.png)
#### Searching by Workflows 
If the documents is part of the control flow, such as `Controlled Documents`, then it can be found inside workflows tab. This tag is only to use that are active participants of said control flow.

![Workflow Documents](/images/temp_assets/workflow.png)

#### Searching by Checkouts
If you are an active participant in a review process, then the document can be found under check outs.
![Checkout Tab](/images/temp_assets/checkout.png)
#### Custom Engine Search
Lastly, this applications supports whoosh search engine. This means that your basic search tab accept whoosh query language.

Full documentation on whoosh query language can be found here: [Whoosh Query Language](https://whoosh.readthedocs.io/en/latest/querylang.html)
Whoosh language highlights:

- Use AND / OR / NOT  in your search:
```console 
EMF AND Anodize NOT titanium 
```

- Search using date ranges:
```console 
date:[20210101 TO 20220715] 
```

- Search using wildcards. "?" replaces a single character, * replace multiple
```console
EMF-8?5 OR EMF-*A 
```

-Emphasizing or emphasizing element of search
```console
SOP^10 EMF^0.5 anodizing
```