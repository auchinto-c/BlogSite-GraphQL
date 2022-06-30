# Blog Site with Graph QL

## Introduction
<hr>
This project showcases demo blog site with GraphQL. We use GraphCMS as the backend platform to manage the content. This website focuses on a gallery view of the posts available in the CMS environment, and the dynamically generated pages for each post.
<br><br>

## Credits
<hr>

|              | Details |
|--------------|--------------------------------------------------------------------------------------------------------------------|
| **Tutorial** | [Blog Site with GraphQL](https://www.youtube.com/watch?v=Dc7LAgqy1_E)                                              |
| **Code**     | [developedbyed - Digital Scribbles](https://github.com/developedbyed/digital-scribbles)                            |

## Brief
<hr>

|                | Details                                                      |
|----------------|--------------------------------------------------------------|
| **Version**    | **v1**                                                       |
| ------------   | ------------                                                 |
| **Demo**       | [Vercel](https://blog-site-graph-ql.vercel.app)              |
| **CMS**        | [GraphCMS](https://graphcms.com)                             |
| **Frameworks** | [GraphQL](https://graphql.org), [NextJs](https://nextjs.org) |

## Procedure
<hr>

1.  Setup the GraphCMS environment.
    a.  Create a new Model called `Post`. Add the following items to it's definition.
        i. Single Line Text - `Title`
        ii. Slug - `Slug`
        iii. Rich Text - `Content`
        iv. Asset Picker - `Cover Image`
        v. Date - `Date Published`
        vi. Relationship - `Two Way Reference - Author (Model)`
    b. Create a new Model called `Author`. Add the following items to it's definition.
        i. Single Line Text - `Name`
        ii. Asset Picker - `Avatar`
        iii. Relationship - `Two Way Reference - Post (Model)`
    c. Add in some dummy data for both of the models, so that it later shows up in our front end.
2.  Create a **next-js** app using `npx create-next-app@latest app-name`
3.  Implement the front end with the following objectives:
    1.  Fetch the entries from graph-cms using graphql
    2.  Showcase them as a gallery view on the landing page
    3.  Generate pages per post, where the content for each post can be displayed
4.  Test these changes in the local environment (`npm run dev`)
5.  Deploy the project to vercel.
<br><br>

## Local Setup
<hr>

1. Clone the repository to your local system.
2. Set the current working directory as `blog-demo` and then run the following command: `npm run dev`. This will deploy the project on the localhost.
<br><br>

## Library and Tools
<hr>

### Language
![HTML 5](https://img.shields.io/badge/html-%23ff6600.svg?style=for-the-badge&logo=html5&logoColor=white)
![CSS 3](https://img.shields.io/badge/css-%230066ff.svg?style=for-the-badge&logo=css3&logoColor=white)
![Javascript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E)

### API Query Language
![GraphQL](https://img.shields.io/badge/graph_ql-%23281f4f.svg?style=for-the-badge&logoColor=white)

### Content Management System
![GraphCMS](https://img.shields.io/badge/graphcms-%23990099.svg?style=for-the-badge&logoColor=white)

### Web Framework
![NextJs](https://img.shields.io/badge/next-js-%2300cc00.svg?style=for-the-badge&logo=next-js&logoColor=white)

### Deployment
![Vercel](https://img.shields.io/badge/vercel-%23000000.svg?style=for-the-badge&logo=vercel&logoColor=white)
<br><br>

## Future Scope
<hr>

1. Here onwards, we can add a more comprehensive client experience for the site. Here are some ideas to include:
   1. Add in NavBars
   2. Add metric features like number of visits, upvotes and downvotes
   3. Add in the feature to comment on the post
   4. Add in the facility to share the post
   5. Add in the facility to search for specific posts, based on genres and other filters
   6. Add a facility to submit a post from the portal instead of the updating entries in cms platform.
2. This entire project can be considered as step to having a personal portfolio and blog site.