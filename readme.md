# React-Laravel News Application

**Table of Contents** 
 - [Assignment](#assignment)
 - [Tech Stack](#techstack)
 - [Platforms](#platforms)
 - [Development](#development)
 - [Developer](#development)

## Assignment
To develop the below features by using React.js, Laravel, MySOL and deploy it on a server (preferable AWS).

**Feature List:**
 - [x] (1) Login
 - [x] (2) Sign up 
 - [x] (3) Edit Profile: 
    - [ ] Exact Location (Google places API) 
        (*Note : Currently storing location as a string only)
 - [x] (3) Profile View
 - [x] (4) New Post 
 - [x] (4) Post view 
 - [x] (4) Like Button
 - [x] (5) Make sure when a user makes a post the other user can see it.
 
**Addition Features Added**
 - [x] Edit Post 
 - [x] Delete Post
 - [x] Advance Editor for post content (ckeditor)
 - [x] Image Upload for Post
 - [x] Pagination for Posts

## TechStack 
 - Laravel 
 - React 
 - Redux
 - MySQL

## Development
Clone the repository. Do the following steps to get it up and running:
1. Set your db configuration in .env
2. `composer install`
3. `npm install`
4. `php artisan migrate`
5. `npm run watch` *(To start React frontend)
6. `php artisan serve` *(To start Laravel backend api)

You can access the application at http://127.0.0.1:8000/

***For react production build** - execute `npm run prod`

## API  

(\*) represents routes which requires authorization header as - Bearer <API TOKEN>

 | Routes | Method | Description | 
 |:----------|:-------------:|:------| 
 | api/login | POST | Login route. | 
 | api/logout | GET | User Logout. | 
 | api/register | POST | User registeration. | 
 | api/check-auth | GET | Authenticate user. | 
 | api/profile | GET | Get user profile. | 
 | api/profile/update | POST | Update user profile. | 
 | api/posts?page= | GET | List all posts. (Returns 10 items per page with pagination data )| 
 | api/posts/:id | GET | Get post by id. | 
 | api/posts | POST | Create new post. | 
 | api/posts/likes | POST | Like post by id. | 
 | api/posts/:id | PUT | Edit post by id. | 
 | *api/posts/:id | DELETE | Delete post by id. |


## Developer 
| [![image](https://avatars3.githubusercontent.com/u/41014321?s=128&v=4)](https://smithgajjar.tech) |
|:-:|
| [![LinkedIn](https://icons.iconarchive.com/icons/danleech/simple/32/linkedin-icon.png)](https://www.linkedin.com/in/smith-gajjar-5a27716b/) [![Portfolio](https://icons.iconarchive.com/icons/dtafalonso/android-lollipop/32/Browser-icon.png)](https://smithgajjar.me) |