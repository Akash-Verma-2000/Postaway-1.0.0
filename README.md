# Postaway Social Media APIs 

Welcome to the engine behind a vibrant social media application! My REST API forms the core of an interactive platform, providing essential functionalities to enhance your social experience. Designed with simplicity and security in mind, this API enables users to seamlessly create, share, and interact with posts and comments. Through robust authentication mechanisms and precise authorization controls, my API ensures that user data remains protected while allowing for personalized engagement. Dive into a world where users can manage their content, connect through comments, and express themselves with likes – all within a safe and controlled digital space.


## Technologies

![HTML](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![Bootstrap](https://img.shields.io/badge/Bootstrap-563D7C?style=for-the-badge&logo=bootstrap&logoColor=white)
![Javascript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Git](https://img.shields.io/badge/GIT-E44C30?style=for-the-badge&logo=git&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white)
![Express.js](https://img.shields.io/badge/Express.js-404D59?style=for-the-badge)


## Authentication & Authorization

- Using JWT tokens for authentication upon login.

- Implement middleware for authorization, ensuring only authorized users can access specific endpoints based on roles and ownership.


## Error Handling

- Implementing meaningful error responses and status codes for various scenarios (e.g., unauthorized access, missing data, server errors).


## API Overview

- **User Authentication**

    - **User Registration**: Allows users to create new accounts by providing necessary details.

    - **User Login**: Enables users to authenticate themselves by logging into their accounts.

- **Posts**:

    - **Get All Posts**: Authenticated users can retrieve all posts available on the platform.

    - **Get Specific Post**: Authenticated users can access a particular post by its ID.

    - **Delete Post**: Users who created the post can delete it.
    
    - **Update Post**: Post creators have the ability to update their posts.

    - **Create Post**: Authenticated users can create new posts.

    - **Get Logged-in User Posts**: Users can retrieve their own posts after logging in.

- **Comments**:

    - **Get Comments for Specific Post**: Authenticated users can view comments related to a specific post.

    - **Delete Comment**: Post owner and comment creator can delete comments.

    - **Update Comment**: Post owner and comment creator can modify comments.

    - **Post Comment**: Authenticated users can add comments to posts.

- **Likes**:

    - **Like/Unlike Post**: Authenticated users can like or unlike specific posts.

    - **Get Likes for Specific Post**: Authenticated users can see the likes on any post.

### Steps to Setup

1. Clone the repository
2. Install dependencies
3. Run the server from the index.js file 
3. The server will start listening on port 4000.


## Project Structure

- **`errorHandler/`**
    - **`application.error.js`** Error class of the APIs
    
- **`features/`**
    
    - **`comment/`**

        - **`comment.controller.js`** All the cotrolling operations of the comments related APIs.

        - **`comment.model.js`** All the data operations of the comments related APIs.

        - **`comment.route.js`** All the routes configurations of the comments related APIs.

    - **`like/`**

        - **`like.controller.js`** All the cotrolling operations of the likes related APIs.

        - **`like.model.js`** All the data operations of the likes related APIs.

        - **`like.route.js`** All the routes configurations of the like related APIs.  

    - **`post/`**

        - **`post.controller.js`** All the cotrolling operations of the post related APIs.

        - **`post.controller.js`** All the data operations of the post related APIs.

        - **`post.route.js`** All the routes configurations of the post related APIs.  
    
    - **`user/`**

        - **`user.controller.js`** All the cotrolling operations of the user related APIs.

        - **`user.controller.js`** All the data operations of the user related APIs.

        - **`user.route.js`** All the routes configurations of the user related APIs.  
        

- **`middleware/`**

    - **`fileUpload.middleware.js`** Middleware for uploading image files.

    - **`jwt.middleware.js`** Authentication token middleware.

    - **`logger.middleware.js`** Middle for logging request URL and request body.


- **`uploads/`**:This folder contains all the uploaded images.

- **`log.txt`** logger.middleware.js file is logging data in this file.

- **`package-lock.json`** This file contains the information about the versions of all the dependencies.

- **`index.js`**: Entry point of the application.

- **`package.json`**: File containing project metadata and dependencies.

- **`README.md`**: File containing complete project details.

- **`swagger.json`** Documentation file of all the APIs.


## API Endpoints


 - ### User Route

    -  User registration

        `POST /api/user/signup` 

    - User login

        `POST /api/user/signin` 


 - ### Post Route

    - Get all posts

      `GET /api/posts/all`

    - Get a specific post by post id

      `GET /api/posts/:id`

    - Get post by user id

      `GET /api/posts/`

    - Create post

      `POST /api/posts/`

    - Delete post by post id

      `DELETE /api/posts/:id`

    - Update post by post id

      `PUT /api/posts/:id`


 - ### Comment Route

    - Get all comments by post id

      `GET /api/comments/:id`

    - Create new comment by post id

      `POST /api/comments/:id`

    - Delete comment by comment id

      `DELETE /api/comments/:id`

    - Update comment by comment id

      `PUT /api/comments/:id`

 - ### Like Route

    - Get all likes by post id

      `GET /api/likes/:id`

    - Toggle like by post id

      `GET /api/likes/toggle/:id`

 - ### Documentation Route

    - Get the compplete API Docs

        `GET /api-docs`


## Author

Akash Verma

## Contact me 

 [![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/akash-verma-09aug2000/)  [![LeetCode](https://img.shields.io/badge/-LeetCode-FFA116?style=for-the-badge&logo=LeetCode&logoColor=black)](https://leetcode.com/Akash_Verma2000/)  [![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:akash.verma217112@gmail.com) 
 [![Naukari](https://img.shields.io/badge/Naukri.com-0A66C2?style=for-the-badge&logo=Naukri.com&logoColor=white)](https://www.naukri.com/mnjuser/profile)
  
## License

This project is licensed under the ISC License.
