steps lesson 02

1. create the base code as usual for redux project
2. create the store
3. create the postsSlice
4. create PostsList.jsx to display the list
5. create AddPostForm.jsx to add post
6. create usersSlice.js
7. create PostAuthor.jsx
8. create TimeAgo.jsx
9. create ReactionButtons.jsx

steps lesson 03

1. install axios
2. set the POSTS_URL
3. create initialState
4. create fetchPosts
5. create extraReducers
6. export the state values
7. update PostList.jsx
   - get all posts values from postsSlice.js
   - use useEffect to fetchPosts using dipatch when postsStatus is idle
   - create variable content
   - update content based on postsStatus
   - create PostsExcerpt
7. create addNewPost
8. update extraReducers
9. update AddPost.jsx
   - update canSave, add checking if the status is idle
   - if canSave, call dispatch -> call addNewPost, unwrap, then, catch
10. in usersSlice.js
   - create USERS_URL const
   - create initialState emptry array
   - create fetchUsers
   - create extraReducers

step lesson 04

1. in postsSlice.js, create the selectPostById function and export it
2. create SinglePostPage.jsx
   - install react-router-dom
   - use useparams to get postId from url
   - call selectpostbyid to get the post
     - wrap the postId with Number
   - create return when !post
   - create return if post available, just like in PostsExcerpt
3. in index.jsx, add routing for the <App />
4. create Layout.jsx
5. update App.jsx to include route for all pages
6. in PostsExcerpt
   - substring the body to 75...
   - add Link before PostAuthor to view post
7. create Header.jsx
   - add logo and nav link to Home and Post
   - add Header in Layout.jsx before main
8. in PostList remove h2 
9. in PostsExcerpt change h3 to h2
10. in SinglePostPage, add edit Link before PostAuthor
11. create EditPostForm.jsx
	- almost similar to AddPost.jsx
    - a long one, refer previous code
12. in postSlices, create updatePost function and add addCase for updatePost
13. style the whole things first
14. create deletePost function in postsSlice
15. add delete post button in EditPostForm

step lesson 05

1. fix from previous lesson, in EditPostForm, in author on change, wrap e.target.value with Number
2. create UsersList.jsx
3. create selectUserById in usersSlice
4. create UserPage.jsx
5. in App.jsx, add route for user for UsersList and UserPage
6. add catch all route
7. in Header.jsx, add link to /user
8. update postSlice
	- remove addPost because not used anymore
	- in initialState add count:0
	- below addReaction add increateCount reducer to increment count
	- create getCount and export
	- remove addPost in exported postsSlice.actions and add increaseCount
9. update Header.jsx
	- get count by calling getCount
	- add button below ul to increase count by calling increaseCount


